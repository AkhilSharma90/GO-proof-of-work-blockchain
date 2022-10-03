Few days back, we created a very simple blockchain on my youtube channel. 
It demonstrated what a blockchain is really well, but blockchains need some consensus mechanism.

In this example, I have shown a very simple POW consensus mechanism.

Uses GO for the same.

To run -

`go run main.go`

Open `http://localhost:8080` in a browser and you will see one block. 

To add blocks, you send a POST request to `localhost:8080` using CURL.
Send a BPM like `{"BPM":75}` in the body of this post request.

`curl -X POST -H "Content-Type: application/json" -d '{"name": "75"}'`

Your terminal will start performing the work.

Then hit the same terminal from a browser and you will an added block. Voila!