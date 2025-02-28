Provide your CLI command here:
jq -r '.order_id' ./transaction-log.txt | xargs -n1 -I {} sh -c 'curl -X GET "https://example.com/api/{}"; echo' >> ./output.txt
