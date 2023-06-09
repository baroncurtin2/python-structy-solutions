# tolerant teams

## Description

Write a function, tolerant_teams, that takes in a list of rivalries as an argument. A rivalry is a pair of people who should not be placed on the same team. The function should return a boolean indicating whether or not it is possible to separate people into two teams, without rivals being on the same team. The two teams formed do not have to be the same size.

## Test Cases

test_00:

```text
tolerant_teams([
  ('philip', 'seb'),
  ('raj', 'nader')
]) # -> True
```

test_01:

```text
tolerant_teams([
  ('philip', 'seb'),
  ('raj', 'nader'),
  ('raj', 'philip'),
  ('seb', 'raj')
]) # -> False
```

test_02:

```text
tolerant_teams([
  ('cindy', 'anj'),
  ('alex', 'matt'),
  ('alex', 'cindy'),
  ('anj', 'matt'),
  ('brando', 'matt')
]) # -> True
```

test_03:

```text
tolerant_teams([
  ('alex', 'anj'),
  ('alex', 'matt'),
  ('alex', 'cindy'),
  ('anj', 'matt'),
  ('brando', 'matt')
]) # -> False
```

test_04:

```text
tolerant_teams([
  ('alan', 'jj'),
  ('betty', 'richard'),
  ('jj', 'simcha'),
  ('richard', 'christine')
]) # -> True
```

test_05:

```text
tolerant_teams([
  ('alan', 'jj'),
  ('betty', 'richard'),
  ('jj', 'simcha'),
  ('richard', 'christine')
]) # -> True
```

test_06:

```text
tolerant_teams([
  ('alan', 'jj'),
  ('jj', 'richard'),
  ('betty', 'richard'),
  ('jj', 'simcha'),
  ('richard', 'christine')
]) # -> True
```

test_07:

```text
tolerant_teams([
  ('alan', 'jj'),
  ('betty', 'richard'),
  ('betty', 'christine'),
  ('jj', 'simcha'),
  ('richard', 'christine')
]) # -> False
```
