# The Blockchain Bar
> Build a custom blockchain in Go.

The full source-code for book: "The Blockchain Way of Programming".

https://web3.coach

## Foreword
Welcome to the blockchain world!

Thank you for your trust and purchase of the full eBook version. You made the right choice of learning blockchain development and expanding your programming career.

Enjoy the ride :)

## How to use this repository
Every chapter has a dedicated branch where you can experiment with the code first-hand.

```git
git branch

> c1_genesis_json
> c2_db_changes_txt
> c3_state_blockchain_component
> c4...
> c5...
```

## Getting Started
1. Open the eBook at Chapter 1
1. Checkout the first chapter's branch

```git
git checkout c1_genesis_json
```

Read, experiment with the code and, most importantly, have fun!

## Blockchain Usage

### Show current program's version
```bash
tbb help
```

### Launch the blockchain and its HTTP API
```
tbb run --datadir=/home/web3coach/.tbb
```

### List all balances
```
curl -X GET http://localhost:8080/balances/list -H 'Content-Type: application/json'
```

### Add a new TX
```
curl -X POST http://localhost:8080/tx/add -H 'Content-Type: application/json' -d '{"from": "andrej","to": "andrej","value": 100,"data": "reward"}'
```

## Compile

To local OS:
```
go install ./cmd/...
```

Cross-compile to Linux:
```
xgo --targets=linux/amd64 ./cmd/tbb
```

## Getting Unstuck
Can't understand why is something done in a particular way or crack your way around a specific chapter's topic?
   
As I promised, you have my full support. You are not alone in this. Write me a DM on LinkedIn, and I will help you figure it out and move forward on your new journey :)
   
[https://www.linkedin.com/in/llukac](https://www.linkedin.com/in/llukac)