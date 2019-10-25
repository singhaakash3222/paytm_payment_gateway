# paytm_payment_gateway
How to install the sample kit on a web server:
1. Copy PaytmKit folder in document root of your server (like /var/www/html)
2. Open config_paytm.php file from the PaytmKit/lib folder and update the below constant values
    - PAYTM_MERCHANT_KEY – Provided by Paytm
     - PAYTM_MERCHANT_MID - Provided by Paytm
      - PAYTM_MERCHANT_WEBSITE - Provided by Paytm
3. PaytmKit folder is having following files:
      - Index.php – Testing transaction through Paytm gateway.
      - pgRedirect.php – This file has the logic of checksum generation and passing all required parameters to Paytm PG.
      - pgResponse.php – This file has the logic for processing PG response after the transaction processing.
       - TxnStatus.php – Testing Status Query API
