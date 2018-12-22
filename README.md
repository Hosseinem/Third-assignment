# Third-assignment
Benchmark analysis of two data structure(Binary Tree, Heap) and two sorting methods(Quick sort, Bubble sort)

This report has been created to show the result of a benchmark analysis undertaken for a project in computer science in Sapienza University. The goal of this report is to show the result of testing the performances of four programs, two of which are methods to accumulate data and the other two are algorithms for sorting numbers in a given list.

First thing to do is to define four classes to keep the track of minimum and maximum, you can find my codes in the link below:

https://github.com/Hosseinem/Third-assignment/blob/master/Codes%20of%20classes

Each class has three methods add(adds an integer to the list), get_min(returns the smallest integer in the list) and get_max(returns the largest integer in the list). For testing the performances I generated 50 lists with random numbers having different lengths, starting from 10 and increasing by 200 up to 10000 then I applied them to each class and measured the time of execution with a function I wrote as "measure_time", in which I used a repetition of 40 times and took the average to be more precise, you can find the codes below: 

https://github.com/Hosseinem/Third-assignment/blob/master/Codes%20to%20measure%20the%20time%20and%20to%20create%20data

I organized the result of the Benchmark analysis in the table below:

|Length|Binary Tree add|Binary Tree get_min|Binary Tree get_max|Heap class add|Heap class get_min|Heap class get_max|Quick sort add|Bubble sort add|
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|10|0.0|0.0|0.0|0.0|0.10001659393310547|0.0|0.0|0.0|
|210|2.198725938796997|1.0014057159423828|0.8001267910003662|0.3006398677825928|0.0|0.29950737953186035|0.6000876426696777|0.9200937747955322|
|410|3.0985355377197266|2.6001393795013428|1.7002403736114502|0.7005631923675537|0.20001530647277832|0.30000805854797363|0.9000897407531738|20.50691509246826|
|610|6.704193353652954|2.000248432159424|2.89955735206604|1.8996775150299072|0.3005385398864746|0.30013322830200195|1.5001296997070312|154.3611557483673|
|810|8.00366997718811|2.1001458168029785|4.100370407104492|1.8008530139923096|0.7032394409179688|0.7008492946624756|1.9001364707946777|616.080828666687|
|1010|6.8009257316589355|3.700411319732666|4.198431968688965|3.0999064445495605|1.0013341903686523|1.1998474597930908|2.1001458168029785|-|
|1210|11.008578538894653|4.10153865814209|7.004666328430176|2.701103687286377|0.7999181747436523|1.0987401008605957|3.7001967430114746|-|
|1410|13.204586505889893|5.698925256729126|6.199860572814941|3.6014795303344727|1.8019258975982666|1.4000117778778076|4.300093650817871|-|
|1610|14.405030012130737|6.6003382205963135|8.100438117980957|4.19996976852417|1.2006521224975586|2.198690176010132|6.601607799530029|-|
|1810|17.70119071006775|5.200415849685669|9.100198745727539|4.398632049560547|1.1001884937286377|0.9005546569824219|5.399966239929199|-|
|2010|17.09904670715332|5.5999040603637695|9.206467866897583|3.6992013454437256|1.5011906623840332|1.3008952140808105|5.2026450634002686|-|
|2210|21.502399444580078|7.606256008148193|11.69847846031189|5.797284841537476|2.7030766010284424|1.7995953559875488|10.001170635223389|-|
|2410|19.7010338306427|9.60279107093811|10.997354984283447|5.199646949768066|1.6011178493499756|1.9997894763946533|6.40026330947876|-|
|2610|23.806077241897583|8.397090435028076|14.501464366912842|7.401525974273682|1.3998985290527344|2.49980092048645|6.400501728057861|-|
|2810|22.60690927505493|9.100133180618286|10.699033737182617|5.400556325912476|2.2992968559265137|2.3992061614990234|5.49958348274231|-|
|3010|26.90560817718506|9.70277190208435|12.399184703826904|8.000034093856812|3.2013773918151855|2.7000367641448975|11.200898885726929|-|
|3210|31.599473953247067|9.900504350662231|14.906609058380127|8.800387382507324|3.899937868118286|2.2996246814727783|11.399662494659424|-|
|3410|27.099531888961792|10.003906488418579|15.204960107803345|7.696640491485596|2.9012680053710938|2.401888370513916|10.20088791847229|-|
|3610|31.701248884201046|11.800116300582886|18.30519437789917|5.301123857498169|1.999819278717041|3.0009567737579346|9.40350890159607|-|
|3810|29.407578706741333|11.000370979309082|17.201828956604004|7.996684312820435|3.502333164215088|3.9012789726257324|16.801053285598755|-|
|4010|35.70551872253418|15.398311614990234|17.201483249664307|8.364766836166382|2.5136232376098633|2.763533592224121|19.29996609687805|-|
|4210|36.80662512779236|15.305638313293457|23.701435327529907|4.516869783401489|1.8003106117248535|2.051568031311035|11.502188444137573|-|
|4410|38.20614218711853|14.198654890060425|23.70840311050415|9.846854209899902|3.1669914722442627|3.398698568344116|15.9015953540802|-|
|4610|43.50077509880066|15.8034086227417|23.002582788467407|8.555513620376587|3.127408027648926|3.239518404006958|16.302621364593506|-|
|4810|38.80382180213928|15.603137016296387|22.09862470626831|11.557692289352417|4.251730442047119|4.204481840133667|18.40118169784546|-|
|5010|45.2073872089386|16.60568118095398|25.200331211090088|13.392210006713867|4.291290044784546|4.7245800495147705|21.10363245010376|-|
|5210|47.70911931991577|16.701078414916992|26.706451177597046|12.297189235687256|4.492354393005371|3.953200578689575|19.803959131240845|-|
|5410|43.80080699920654|16.40201210975647|23.208892345428467|11.737102270126343|4.093974828720093|4.567044973373413|20.001107454299927|-|
|5610|45.90483903884888|14.40061330795288|24.908214807510376|16.728204488754272|5.616545677185059|5.868154764175415|28.677421808242798|-|
|5810|51.5935480594635|18.60162615776062|29.310840368270874|10.751897096633911|4.014021158218384|4.3542444705963135|17.88705587387085|-|
|6010|49.104851484298706|19.297945499420166|26.508021354675293|17.132872343063354|5.256998538970947|5.289942026138306|15.881097316741942|-|
|6210|41.11546277999878|16.001874208450317|23.09812307357788|13.491678237915039|4.619109630584717|5.056500434875488|20.02413272857666|-|
|6410|46.711939573287964|21.608495712280273|24.51031804084778|13.759994506835938|4.302722215652466|4.836541414260864|18.501412868499756|-|
|6610|51.40041708946228|18.20785403251648|24.803954362869263|14.063060283660889|4.525309801101685|4.11418080329895|32.60306715965271|-|
|6810|57.20513463020325|22.30094075202942|32.80748128890991|17.64478087425232|5.022287368774414|6.74012303352356|32.80104994773865|-|
|7010|63.50428462028504|23.21009635925293|30.50137758255005|18.02469491958618|5.176520347595215|4.7550201416015625|23.70373010635376|-|
|7210|54.24461364746094|21.784943342208862|29.3298602104187|13.170069456100464|5.326735973358154|4.5135498046875|31.905812025070187|-|
|7410|69.46619749069214|26.801949739456177|38.78868818283081|13.430190086364746|5.3742170333862305|5.909919738769531|27.88558006286621|-|
|7610|65.58746695518494|25.522351264953613|36.47589087486267|19.273710250854492|5.587196350097656|7.162082195281982|23.627275228500366|-|
|7810|68.62491965293884|26.695150136947632|34.14129018783569|17.701327800750732|6.700152158737183|6.698960065841675|28.21981906890869|-|
|8010|60.242581367492676|24.33273196220398|35.29965281486511|17.700648307800293|5.899834632873535|5.000263452529907|33.70514512062073|-|
|8210|67.52162575721741|27.343088388442993|37.25268244743347|18.500930070877075|6.103581190109253|7.797682285308838|32.002902030944824|-|
|8410|70.03695964813232|27.560532093048096|40.14279246330261|22.001612186431885|6.803321838378906|6.2025368213653564|25.78657865524292|-|
|8610|73.36938381195068|29.383832216262817|41.06736779212952|14.402449131011963|5.801022052764893|5.299234390258789|29.200655221939087|-|
|8810|72.8125512599945|27.227038145065308|37.87321448326111|17.99381375312805|6.001335382461548|9.30861234664917|34.43678021430969|-|
|9010|75.27180910110474|30.610370635986328|42.03199744224548|25.405067205429077|6.39958381652832|7.300359010696411|36.704808473587036|-|
|9210|76.85397863388062|31.273269653320312|42.60643720626831|22.499412298202515|7.301586866378784|8.804923295974731|35.30150651931763|-|
|9410|78.28697562217712|32.70401954650879|40.31745791435242|18.39936375617981|6.099283695220947|7.0022642612457275|39.50051665306091|-|
|9610|85.46692132949829|28.99869680404663|42.7324652671814|28.198570013046265|8.503472805023193|8.202534914016724|36.905014514923096|-|
|9810|85.20827889442444|32.21052289009094|46.89839482307434|19.8022723197937|5.8979034423828125|7.6024651527404785|33.406275510787964|-|

The codes of get_min and get_max methods in Bubble sort and Quick sort are the same and the time to get the firts or last element after sorting them is almost zero, so I just measured the add method which illustrates the proper alteration of the performance of sorting algorithms while increasing the length of the given lists.


<p align="center"><img src = "https://github.com/Hosseinem/Third-assignment/blob/master/1.png" width = "400" height = "320"/><img src = "https://github.com/Hosseinem/Third-assignment/blob/master/2.png" width = "400" height = "320"/>

Consequently, by increasing the length of the lists,the Bubble sort is gets much more slower.As a matter of fact, Bubble sort was too slow that I had to put it in seconds instead of milliseconds and also put only the first 5 lists, you can see the major difference in the figure below(Note that Bubble sort's line is in the middle just for comparison, the scale is different both in time and length of the lists):

<p align="center"><img src = "https://github.com/Hosseinem/Third-assignment/blob/master/9.png" width = "550" height = "350"/>


In the following figures you can see the performances of Binary Tree and Heap:

<p align="center"><img src = "https://github.com/Hosseinem/Third-assignment/blob/master/3.png" width = "400" height = "320"/><img src = "https://github.com/Hosseinem/Third-assignment/blob/master/4.png" width = "400" height = "320"/>

In comparison, Heap performance is much faster than Binary Tree due to the fact that in Heap we add the new element at the last position and it doesn't have any left or right ordering such as Binary tree.

<p align="center"><img src = "https://github.com/Hosseinem/Third-assignment/blob/master/5.png" width = "280" height = "230"/><img src = "https://github.com/Hosseinem/Third-assignment/blob/master/6.png" width = "280" height = "230"/><img src = "https://github.com/Hosseinem/Third-assignment/blob/master/7.png" width = "280" height = "230"/>



In conclusion, the comparison of the three programs all together that ilustrates the fact that Heap is the fastest and then Quick sort and Binary Tree and finally Bubble sort is the slowest one with a major difference.


<p align="center"><img src = "https://github.com/Hosseinem/Third-assignment/blob/master/8.png" width = "450" height = "350"/>


# System information:

Python version     :   3.7.1

Operating System   :   Windows 10 Enterprise 64-bit 

Processor          :   Intel(R) Core(TM) i7-4600U CPU@ 2.10GHz (4 CPUs), =2.7GHz

Memory             :   16384MB RAM 

