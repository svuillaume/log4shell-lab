### https://www.cvedetails.com/vulnerability-list/vendor_id-45/product_id-37215/version_id-677193/year-2021/Apache-Log4j-2.14.1.html



# Build project
mvn clean install

# Run vulnerable server
mvn exec:java -Dexec.mainClass="demo.VulnerableServer"

or

# Run vulnerable server as background process
nohup mvn exec:java -Dexec.mainClass="demo.VulnerableServer" &

# Optional: run callback monitor
mvn exec:java -Dexec.mainClass="demo.CallbackMonitor"
