Demonstraiting a break of including codeception configurations + using groups in included suites in codeception patch release 4.1.24.
Codeception 5 behaves same as ^4.1.24

1. run `composer update`
2. note running multiple variants on groups and suites are working with codeception 4.1.23
  - `vendor/bin/codecept run`
  - `vendor/bin/codecept run -g unit1`
  - `vendor/bin/codecept run -c src/Core`
  - `vendor/bin/codecept run -c src/Core -g unit1`
3. change `codeception/codeception` constraint in composer.json to `^5` or `4.1.24` (same result) and execute `composer update`
4. run any of the above codeception commands. All are failing.
