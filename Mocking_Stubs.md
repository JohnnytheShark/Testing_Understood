# Terminology Clarified

| Category | Pattern | Purpose | Uses |
| --- | --- | --- | --- |
| Stub | Test Double | Generic name for stubs and mocks | I also use the term fake | 
| | Dummy Object | Used to specify the values to be used in tests when the only usage is as irrelevant arguments of SUT method calls | Send as a parameter to the entry point or as the arrange part of the AAA pattern. | 
| | Test Stub | Used to verify logic independently when it depends on indirect inputs from other software components | Inject as a dependency, and configure it to return specific values or behavior into the SUT | 
| Mock | Test Spy | Used to verify logic independently when it has indirect outputs to other software components | Override a single function on a real object, and verify that the fake function was called as expected.  | 
| | Mock Object | Used to verifiy logic independently when it depends on indirect outputs to other software components | Inejct the fake as a dependency into the SUT, and verify that the fake was called as expected | 

