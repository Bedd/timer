# README
[![Build Status](https://travis-ci.org/Bedd/timer.svg?branch=master)](https://travis-ci.org/Bedd/timer) [![Latest Stable Version](https://poser.pugx.org/Bedd/timer/v/stable)](https://packagist.org/packages/Bedd/timer) [![Total Downloads](https://poser.pugx.org/Bedd/timer/downloads)](https://packagist.org/packages/Bedd/timer) [![Latest Unstable Version](https://poser.pugx.org/Bedd/timer/v/unstable)](https://packagist.org/packages/Bedd/timer) [![License](https://poser.pugx.org/Bedd/timer/license)](https://packagist.org/packages/Bedd/timer)[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/Bedd/timer/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/Bedd/timer/?branch=master)

## Installation
The best way to install this library is to use [composer](https://getcomposer.org/).

```json
{
    "require": {
        "bedd/timer": "1.*"
    }
}
```

## Usage
```php
$t = new Bedd\Timer\Timer();
$t->start();

// your process
sleep(3);

$t->end();
print_r($t->getSummary());
```

## Output
```php
Array
(
    [status] => 3
    [start] => 1488831973.2328
    [end] => 1488831976.2334
    [total] => 3.0005979537964
    [paused] => 0
    [laps] => Array
        (
            [0] => Array
                (
                    [name] => start
                    [start] => 1488831973.2328
                    [end] => 1488831976.2334
                    [total] => 3.0006039142609
                )
        )
)
```

## License
This library is available under the [MIT license](LICENSE).