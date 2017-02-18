
```
import demoapp
import unittest


class FlaskTestCase(unittest.TestCase):

    def setUp(self):
        demoapp.app.config['TESTING'] = True
        self.app = demoapp.app.test_client()

    def test_correct_http_response(self):
        resp = self.app.get('/hello/world')
        self.assertEquals(resp.status_code, 200)

    def test_correct_content(self):
        resp = self.app.get('/hello/world')
        self.assertEquals(resp.data, '"Hello World!"\n')

    def test_universe_correct_http_response(self):
        resp = self.app.get('/hello/universe')
        self.assertEquals(resp.status_code, 200)

    def test_universe_correct_content(self):
        resp = self.app.get('/hello/universe')
        self.assertEquals(resp.data, '"Hello Universe!"\n')

    def tearDown(self):
        pass

if __name__ == '__main__':
    unittest.main()

```

