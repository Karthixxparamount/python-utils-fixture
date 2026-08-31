# python-utils-fixture

One small function, tested with pytest.

```python
from stats_utils import average

average([2, 4, 6])  # 4
```

Deliberately minimal: this repo exists to exercise a real `pip install` +
real pytest run inside a sandbox, alongside a JS repo, at the same time --
proving each run provisions its own sandbox image. `average()` currently
has a real, deliberately planted bug (divides by `len(numbers) + 1`) --
`pytest` fails on it as-is. Noting that plainly rather than presenting it
as something found in the wild.
