# bitmex-api-php 
Bitmex api ile bağlantı kurulabilmesi için local php dosyası. index.php olarak kullanarak diğer stratejilerinizi inculude ederek kullanabilirsiniz. Localhost da zamanlanmış görev olarak sıralı işlem yapılabilmektedir.

Get API keys from https://www.bitmex.com/app/apiKeys

HTTP Keep-Alive: BitMex says that "When using HTTP Keep-Alive, request/response round-trip time will be identical to Websocket"

## Usage Example
    <?php
    require_once ("BitMex.php");
    
    $key = "xxxxxxxxxxxxxxxxxxxxxx";
    $secret = "yyyyyyyyyyyyyyyyyyyyyy";

    $bitmex = new BitMex($key,$secret);
    
    var_dump($bitmex->createOrder("Limit","Sell",50000,1000));
    ?>


