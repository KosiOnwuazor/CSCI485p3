# File Decryption and HTTP Upload

This project demonstrates how to decrypt a file and send it to a remote server via HTTP request. It includes implementations in both C/C++ with libcurl and Rust with reqwest.

## Features

- Decrypts a file using AES encryption.
- Sends the decrypted file to a remote server via HTTP POST request.

## Dependencies

### C/C++ (libcurl)

- libcurl: For handling HTTP requests.

### Rust (reqwest)

- reqwest: For handling HTTP requests.

## Usage

### C/C++ (libcurl)

1. Ensure you have libcurl installed on your system.
2. Compile the C/C++ code using a suitable compiler (e.g., GCC).
    ```bash
    gcc -o file_decryption_c file_decryption_c.c -lcurl
    ```
3. Run the compiled executable.
    ```bash
    ./file_decryption_c
    ```

### Rust (reqwest)

1. Add reqwest to your Cargo.toml dependencies.
    ```toml
    [dependencies]
    reqwest = "0.11"
    ```
2. Run the Rust code using Cargo.
    ```bash
    cargo run --release
    ```

## Configuration

- Replace the placeholder URL (`http://example.com/upload`) in the source code with the actual URL of your server.

## File Structure

- `file_decryption_c.c`: C source code for file decryption and HTTP upload using libcurl.
- `file_decryption_rust.rs`: Rust source code for file decryption and HTTP upload using reqwest.
- `secret_file.txt`: File containing the decryption key.
- `special_file.txt`: Encrypted file to be decrypted and uploaded.
- `decrypted_special_file.txt`: Decrypted file generated after decryption.
- `README.md`: Documentation file.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
