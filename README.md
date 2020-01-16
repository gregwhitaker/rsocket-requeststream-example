# rsocket-requeststream-example
An example of using the request-stream interaction model in [RSocket](http://rsocket.io).

## Building the Example
Run the following command to build the example:

    ./gradlew clean build
    
## Running the Example
Follow the steps below to run the example:

1. Run the following command to start the `count-service`:

        ./gradlew :count-service:run
        
2. In a new terminal, run the following command to start the `count-client` and request integers `1` to `10`:

        ./gradlew :count-client:run
        
    If successful, you will see the following in the terminal:

        > Task :count-client:run
        [reactor-tcp-nio-1] INFO example.count.client.CountClient - Received: 1
        [reactor-tcp-nio-1] INFO example.count.client.CountClient - Received: 2
        [reactor-tcp-nio-1] INFO example.count.client.CountClient - Received: 3
        [reactor-tcp-nio-1] INFO example.count.client.CountClient - Received: 4
        [reactor-tcp-nio-1] INFO example.count.client.CountClient - Received: 5
        [reactor-tcp-nio-1] INFO example.count.client.CountClient - Received: 6
        [reactor-tcp-nio-1] INFO example.count.client.CountClient - Received: 7
        [reactor-tcp-nio-1] INFO example.count.client.CountClient - Received: 8
        [reactor-tcp-nio-1] INFO example.count.client.CountClient - Received: 9
        [reactor-tcp-nio-1] INFO example.count.client.CountClient - Received: 10
        
## Bugs and Feedback
For bugs, questions, and discussions please use the [Github Issues](https://github.com/gregwhitaker/rsocket-requeststream-example/issues).

## License
MIT License

Copyright (c) 2020 Greg Whitaker

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.