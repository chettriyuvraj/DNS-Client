# DNS-Client

A simple client to query DNS servers and parse their response.

As far as protocols go, DNS is pretty clean. This client is not to demonstrate any network wizardry, but just an assurance that I can fiddle around with network protocols and find my way
around :)

- Since this was quite long ago, I am too lazy to implement the command line. If you want to play around with the query, go to the main function in _dns.go_ and manually modify the hex DNS query.
- [Original repository folder](https://github.com/bradfield-csi-5/chettriyuvraj/tree/main/BradfieldCSI/Networks/Prework-2-DNS) if you want to have a look at the commit history.
- The default query is for _example.com_

## Usage

- Generate the binary using _go build_
- Run the binary ./dns

## Output

- I ended up creating a beat-up replica of dig's output, with some fields missing

- <img width="1021" alt="image" src="https://github.com/chettriyuvraj/DNS-Client/assets/32122172/fccb0bec-a014-41a5-a6f0-a4e109c592b6">

- Original _dig_ output in comparison

- <img width="505" alt="image" src="https://github.com/chettriyuvraj/DNS-Client/assets/32122172/6837c4f1-edd2-4c8d-adaf-e185075344f6">


