FROM parrotsec/security

RUN cd home
RUN wget https://golang.org/dl/go1.17.3.linux-amd64.tar.gz && \ 
	tar -C /usr/local -xzf go1.17.3.linux-amd64.tar.gz && \ 
	rm go1.17.3.linux-amd64.tar.gz 

ENV GOPATH="$pwd/.go"
ENV PATH="$PATH:/usr/local/go/bin:$GOPATH/bin"

RUN go install github.com/OJ/gobuster/v3@latest