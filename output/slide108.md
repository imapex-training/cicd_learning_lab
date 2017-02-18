
```
from flask import Flask, request
from flask_restful import Resource, Api, reqparse


app = Flask(__name__)
app = Flask(__name__)
api = Api(app)

class HelloWorld(Resource):
    def get(self):
        text = "Hello World!"
        return text

api.add_resource(HelloWorld, '/hello/world')

class HelloUniverse(Resource):
    def get(self):
        text = "Hello Universe!"
        return text

api.add_resource(HelloUniverse, '/hello/universe')

if __name__ == '__main__':
    # Run Flask
    app.run(debug=True, host='0.0.0.0', port=int("5000"))

```

