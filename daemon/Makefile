all:  gc gofmt doc #gccgo

gc:
	go install -v 

gofmt:
	gofmt -w *.go

GCCGO=gccgo -gccgoflags '-static-libgcc -O3'

gccgo:
	go install -v -compiler $(GCCGO)

clean:

doc:
	godoc github.com/barnex/mumax-daemon/daemon > README
