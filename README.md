## Reference
  https://github.com/loadimpact/k6
## Observation
  - `k6 run -u=1 -i=1  <filename>.js`
  - Runs for 1 iteration by 1 user
  - `k6 run -u=2 -i=5  <filename>.js`
  - Runs for 5 iterations and shared by 2 user that is only 5 iteration will be performed and randomly and user could 
  run in those iterations which means if there are 1 API call within the test it will be called 5 times.
  - Every user is isolated with other.
