# Shell-Reverse

1. **Compile the code**: Save the code in a file, for example, `reverse_shell_server.c`. Then, open a terminal, navigate to the directory where the file is located, and compile it using a C compiler like `gcc`. Here's the command:

    ```bash
    gcc reverse_shell_server.c -o reverse_shell_server
    ```

    This command will compile the code and generate an executable file named `reverse_shell_server`.

2. **Run the server**: Execute the compiled program by running the following command in the terminal:

    ```bash
    ./reverse_shell_server
    ```

    This will start the reverse shell server, which will listen for incoming connections on the specified port.

3. **Connect to the server**: You can use any tool capable of establishing TCP connections, such as `netcat` (`nc`) or a programming language like Python. For example, if you want to connect using `netcat`, use the following command:

    ```bash
    nc <server_ip> <server_port>
    ```

    Replace `<server_ip>` with the IP address of the server where the reverse shell server is running, and `<server_port>` with the port number specified in the code (in this case, `12345`).

4. **Interact with the shell**: Once the connection is established, you can interact with the shell by typing commands into the client terminal. The server will execute these commands on its system and send the output back to the client.

5. **Close the connection**: To close the connection, simply type `exit` or `Ctrl+C` in the client terminal.

Remember that the server and client need to be on the same network or reachable network-wise. Also, ensure that the server's firewall allows incoming connections on the specified port.
