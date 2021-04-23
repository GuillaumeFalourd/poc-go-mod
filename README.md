# poc-go-mod

Repository created following [the Golang Tutorial: Create a Go module](https://golang.org/doc/tutorial/create-module)

## How to use the repository code?

In the `/hello` directory, run:

`go run .`

The output should be something like:

```bash
map[Darrin:Hail, Darrin! Well met! Gladys:Hi, Gladys. Welcome! Samantha:Hail, Samantha! Well met!]
```

## How to test the repository code?

In the `/greetings` directory, run:

`go test`

The output should be something like:

```bash
PASS
ok      example.com/greetings   0.364s
```

Or run:

`go test -v`

To get this output:

```bash
=== RUN   TestHelloName
--- PASS: TestHelloName (0.00s)
=== RUN   TestHelloEmpty
--- PASS: TestHelloEmpty (0.00s)
PASS
ok      example.com/greetings   0.372s
```

## How to compile?

On the `/hello` directory, run: 

`go build`

And test the created binary running:

`./hello`

The output should be something like:

```bash
map[Darrin:Hail, Darrin! Well met! Gladys:Hi, Gladys. Welcome! Samantha:Hail, Samantha! Well met!]
```

*Note: Discover the Go install path, where the go command will install the current package.You can discover the install path by running the go list command, as in the following example:*

`go list -f '{{.Target}}'`
