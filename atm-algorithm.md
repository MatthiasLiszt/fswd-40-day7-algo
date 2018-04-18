# ATM algorithm

begin:

PRINT "PLEASE ENTER AMOUNT AS MULTIPLE OF TEN"

input amount

IF amount is not a multiple of ten goto begin

IF amount is not payable then goto notpayable

curAmount=amount

payout:

IF curAmount > 100 then 

   pay out 100
   
   curAmount=curAmount-100
   
   goto payout

IF curAmount > 50 then 

   pay out 50
   
   curAmount=curAmount-50
   
   goto payout

IF curAmount > 20 then 

   pay out 20
   
   curAmount=curAmount-20
   
   goto payout

IF curAmount > 10 then 

   pay out 10
   
   curAmount=curAmount-10
   
   goto payout

PRINT "THANKS FOR YOUR VISIT"

delay

goto begin


notpayable: 

PRINT "AMOUNT CAN NOT BE PAID"

delay

goto begin
