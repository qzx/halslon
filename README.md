# Halslon datascraper

$ ./halslon | jq '.props.pageProps.page.body[0].primary.data' | sed 's/\\//g' | sed 's/^\"//' | sed 's/\"$//' | jq
