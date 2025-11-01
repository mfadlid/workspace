1. Check the connection time required to establish a TCP connection to the host/port
  ```
  curl -s -o /dev/null -w "Connect: %{time_connect}s\n" http://<ip-database>:<port-database>
  ```
  Example:
  ```
  curl -s -o /dev/null -w "Connect: %{time_connect}s\n" http://172.18.19.211:5432
  ```

Run the command from within the node.
