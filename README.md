Sogou-Translate [![Build Status](https://travis-ci.org/imWildCat/sogou-translate.svg?branch=master)](https://travis-ci.org/imWildCat/sogou-translate) [![codecov](https://codecov.io/gh/imWildCat/sogou-translate/branch/master/graph/badge.svg)](https://codecov.io/gh/imWildCat/sogou-translate) [![PyPI version](https://badge.fury.io/py/sogou-translate.svg)](https://badge.fury.io/py/sogou-translate)
===

The Python wrapper for [Sogou Translate API](http://deepi.sogou.com/docs/fanyiDoc). Only **Python 3.6** is supported.

![sogou_translate_logo](https://user-images.githubusercontent.com/2396817/38472358-b1b2aa96-3b76-11e8-85ec-bbd7b47fc3a8.png)

## Get started
You could install this library using `pip`:

```shell
pip install sogou-translate
```

Note: You might have to [apply for the keys](http://deepi.sogou.com/docs/fanyiQa) in order to use the service. If you wish to have a brief demo of this service, you could use the demo keys mentioned in the related web pages.

## Example usage
```python
from sogou_translate import SogouTranslate, SogouLanguages

trans = SogouTranslate('[Your pid]', '[Your secret key]')

en_text = 'Hello, world!'
zh_text = trans.translate(en_text, from_language=SogouLanguages.EN, to_language=SogouLanguages.ZH_CHS)
print(zh_text) # '你好，世界！'
```

## License

The code is licensed under DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE. For more details, read the [LICENSE](./LICENSE) file.