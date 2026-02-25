# Build project
mvn clean install

# Run vulnerable server
mvn exec:java -Dexec.mainClass="demo.VulnerableServer"

or

# Run vulnerable server as background process
nohup mvn exec:java -Dexec.mainClass="demo.VulnerableServer" &

# Optional: run callback monitor
mvn exec:java -Dexec.mainClass="demo.CallbackMonitor"
