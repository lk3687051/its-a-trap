# ItsATrap!

## TODO

- Add option to throw all messages through nats. this will allow multiple receivers.
 
 `1. trap -> 2. encode to json -> 3. throw to nats <- 4. receive from nats -> 5. buffer -> 6. flush to db`
 
 The process should be able to run in 3 modes.
	1. Trap to buffer to db. (all in one without nats)
        2. Trap to nats (a single process)
        3. From nats to buffer to db (a single process)
  2 & 3 would do the work of 1 with nats in the middle

- Add index option

. . . . . . . . . . . . . . . . _,,,--~~~~~~~~--,_
. . . . . . . . . . . . . . ,-' : : : :::: :::: :: : : : : :º '-, ITS A TRAP!
. . . . . . . . . . . . .,-' :: : : :::: :::: :::: :::: : : :o : '-,
. . . . . . . . . . . ,-' :: ::: :: : : :: :::: :::: :: : : : : :O '-,
. . . . . . . . . .,-' : :: :: :: :: :: : : : : : , : : :º :::: :::: ::';
. . . . . . . . .,-' / / : :: :: :: :: : : :::: :::-, ;; ;; ;; ;; ;; ;; ;\
. . . . . . . . /,-',' :: : : : : : : : : :: :: :: : '-, ;; ;; ;; ;; ;; ;;|
. . . . . . . /,',-' :: :: :: :: :: :: :: : ::_,-~~,_'-, ;; ;; ;; ;; |
. . . . . _/ :,' :/ :: :: :: : : :: :: _,-'/ : ,-';'-'''''~-, ;; ;; ;;,'
. . . ,-' / : : : : : : ,-''' : : :,--'' :|| /,-'-'--'''__,''' \ ;; ;,-'/
. . . \ :/,, : : : _,-' --,,_ : : \ :\ ||/ /,-'-'x### ::\ \ ;;/
. . . . \/ /---'''' : \ #\ : :\ : : \ :\ \| | : (O##º : :/ /-''
. . . . /,'____ : :\ '-#\ : \, : :\ :\ \ \ : '-,___,-',-`-,,
. . . . ' ) : : : :''''--,,--,,,,,,¯ \ \ :: ::--,,_''-,,'''¯ :'- :'-,
. . . . .) : : : : : : ,, : ''''~~~~' \ :: :: :: :'''''¯ :: ,-' :,/\
. . . . .\,/ /|\\| | :/ / : : : : : : : ,'-, :: :: :: :: ::,--'' :,-' \ \
. . . . .\\'|\\ \|/ '/ / :: :_--,, : , | )'; :: :: :: :,-'' : ,-' : : :\ \,
. . . ./¯ :| \ |\ : |/\ :: ::----, :\/ :|/ :: :: ,-'' : :,-' : : : : : : ''-,,
. . ..| : : :/ ''-(, :: :: :: '''''~,,,,,'' :: ,-'' : :,-' : : : : : : : : :,-'''\\
. ,-' : : : | : : '') : : :¯''''~-,: : ,--''' : :,-'' : : : : : : : : : ,-' :¯'''''-,_ .
./ : : : : :'-, :: | :: :: :: _,,-''''¯ : ,--'' : : : : : : : : : : : / : : : : : : :''-,
/ : : : : : -, :¯'''''''''''¯ : : _,,-~'' : : : : : : : : : : : : : :| : : : : : : : : :
: : : : : : : :¯''~~~~~~''' : : : : : : : : : : : : : : : : : : | : : : : : : : : :
