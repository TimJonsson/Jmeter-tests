Some simple tests using Jmeter on the public api https://airportgap.dev-tester.com/docs

Thread group of 10 testing 4 different endpoints and verifying that the response code is [200](https://github.com/TimJonsson/Jmeter-tests/blob/main/jmeter/airportGapTests.jmx#L37), doesn't respond in longer than [5 seconds](https://github.com/TimJonsson/Jmeter-tests/blob/main/jmeter/airportGapTests.jmx#L46) and is not bigger than [10000 bytes](https://github.com/TimJonsson/Jmeter-tests/blob/main/jmeter/airportGapTests.jmx#L31)

The tests are integrated to [Github actions](https://github.com/TimJonsson/Jmeter-tests/blob/main/.github/workflows/jmeter-tests.yml) and are run using https://github.com/TimJonsson/PerfAction where I added functionality to provide my own test results file. Waiting approval on my [pull request](https://github.com/QAInsights/PerfAction/pull/17) in the main repository. 
