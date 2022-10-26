# Mission-to-Mars

### TypeError                                 Traceback (most recent call last)
Input In [3], in <cell line: 2>()
      1 executable_path = {'executable_path': ChromeDriverManager().install()}
----> 2 browser = Browser('chrome', **executable_path, headless=False)

File ~\anaconda3\lib\site-packages\splinter\browser.py:121, in Browser(driver_name, retry_count, *args, **kwargs)
    118 except KeyError:
    119     raise DriverNotFoundError("No driver for %s" % driver_name)
--> 121 return get_driver(driver, retry_count=retry_count, *args, **kwargs)

File ~\anaconda3\lib\site-packages\splinter\browser.py:92, in get_driver(driver, retry_count, *args, **kwargs)
     90 for _ in range(retry_count):
     91     try:
---> 92         return driver(*args, **kwargs)
     93     except driver_exceptions as e:
     94         err = e

TypeError: 'NoneType' object is not callable
