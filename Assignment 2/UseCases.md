| Use Case | Primary Actor |      Precondition      |    Postcondition    |   Technical note   |                            Main scenario                                 |                               Alternate Scenarios                          |
|:--------:|:-------------:|------------------------|---------------------|--------------------|--------------------------------------------------------------------------|----------------------------------------------------------------------------|
|1|Admin|None|<ul><li>A web server has been started</li><li>A note in the access log was written, that the server was started</li></ul>|None|<ol><li>Starts when an administrator wants to start the server.</li><li>System asks for socket port number and shared resource container</li><li>The administrator provides a socket port number and a shared resource container</li><li>System starts a web server on the given port and presents that the server was started and writes a note in the access log.</li></ol>|<ul><li>4a. The web server could not be started due to socket was taken<ol><li>System presents an error message: “Socket XX was taken” (XX is the socket number, Example “80”)</li><li>Exit Use Case</li></ol></li><li>4b. The web server could not be started due restriction on the shared resource container<ol><li>System presents an error message: “No access to folder XX” (XX is the shared resource container provided, Example “\var\www”)</li><li>Exit Use Case</li></ol></li><li>4c. The access log could not be written to<ol><li>System presents an error message. “Cannot write to server log file log.txt”</li><li>Exit Use Case</li></ol></li></ul>|






<li><ol><li></li><li></li></ol></li>
