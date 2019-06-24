# QUnit

## 官方資料

- [Qunit 官網](https://qunitjs.com/)
- [QUnit Github repository](https://github.com/qunitjs/qunit)

## 其他資訊

Npm 套件名稱 : qunit 和 qunitjs 關係, 在 Qunit 2.4.1 以前的套件名稱為 qunitjs 他和現在的 cli 不同, 所以要用 qunit 2.4.1 版本以前的資訊採用 qunitjs, 之後的安裝 qunit 

## 安裝 

using npm isntallation

    $ npm install --save-dev qunit

## Demo Code :

    <!DOCTYPE html>
    <html lang="en-us">

    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>Title Page</title>
        <!-- QUnit CSS -->
        <link href="vendor/qunit/qunit.css" rel="stylesheet">
        <!-- Bootstrap CSS -->
        <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
    </head>

    <body>
        <h1 class="text-center">My Test</h1>
        <div id="qunit"></div>
        <div id="qunit-fixture"></div>
        <!-- QUnit JavaScript -->
        <script src="vendor/qunit/qunit.js"></script>
        <!-- jQuery -->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
        <!-- Bootstrap JavaScript -->
        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>

        <script>
            let arr = ['react', 'angular', 'vue'];
            QUnit.test("Origin testing", function (assert) {
                assert.ok(arr.indexOf('angular') !== -1 , 'angular existed');
            });
            QUnit.test("ES 7 feature testing", function (assert) {
                assert.ok(arr.includes('angular'), 'angular existed');
            });
        </script>
    </body>
    </html>
