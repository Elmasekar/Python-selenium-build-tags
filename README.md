# How to add build tags to automation tests in Python-selenium on [LambdaTest](https://www.lambdatest.com/?utm_source=github&utm_medium=repo&utm_campaign=Python-selenium-tags)

If you want to add build tags to group builds in Python-selenium on LambdaTest, you can follow the steps below. You can refer to sample test repo [here](https://github.com/LambdaTest/python-selenium-sample).

# Steps
With LambdaTest, you can group your test builds with Build tags. These are added for tests by setting the tags in `buildTags` capability. The code below illustrates the usage:

```python
desired_caps = {
            'LT:Options': {
                "build": "Python Demo",  # Change your build name here
                "name": "Python Demo Test",  # Change your test name here
                "platformName": "Windows 11",
                "selenium_version": "4.0.0",
                "buildTags": ["test-build1","test-build2"]   #change build tags here      
            },
            "browserName": "Chrome",
            "browserVersion": "98.0",
        }

```

### Run your test

```bash
python lambdatest.py
```

# Links:

[LambdaTest Community](http://community.lambdatest.com/)

