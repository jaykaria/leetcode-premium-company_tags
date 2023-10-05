jq is a lightweight and flexible command-line JSON processor

brew install jq




Clone this repo where companyTags.json exists and run (pass the company name)

cat companyTags.json | jq -r 'to_entries[] | select(.value | index("Apple")) | .key' 
