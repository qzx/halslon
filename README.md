# Halslon datascraper

$ wget https://github.com/qzx/halslon/blob/main/halslon  
$ ./halslon | jq '.props.pageProps.page.body[0].primary.data' | sed 's/\\//g' | sed 's/^\"//' | sed 's/\"$//' | jq
