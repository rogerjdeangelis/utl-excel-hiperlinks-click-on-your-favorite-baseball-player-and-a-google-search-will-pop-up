# utl-excel-hiperlinks-click-on-your-favorite-baseball-player-and-a-google-search-will-pop-up
Excel hiperlinks click on your favorite baseball player and a google search will pop up 
    Excel hiperlinks click on your favorite baseball player and a google search will pop up                                                              
                                                                                                                                                         
    github                                                                                                                                               
    https://tinyurl.com/yxsdsfaz                                                                                                                         
    https://github.com/rogerjdeangelis/utl-excel-hiperlinks-click-on-your-favorite-baseball-player-and-a-google-search-will-pop-up                       
                                                                                                                                                         
    Cynthia_sas                                                                                                                                          
    https://communities.sas.com/t5/user/viewprofilepage/user-id/13549                                                                                    
                                                                                                                                                         
    SAS Forum                                                                                                                                            
    https://tinyurl.com/y5odnqot                                                                                                                         
    https://communities.sas.com/t5/ODS-and-Base-Reporting/Hyperlink-from-ODS-Excel-to-external/td-p/579186                                               
                                                                                                                                                         
    related repo                                                                                                                                         
    https://github.com/rogerjdeangelis/utl_creating_www_hyperlinks_in_ods_excel                                                                          
                                                                                                                                                         
    /*                   _                                                                                                                               
    (_)_ __  _ __  _   _| |_                                                                                                                             
    | | `_ \| `_ \| | | | __|                                                                                                                            
    | | | | | |_) | |_| | |_                                                                                                                             
    |_|_| |_| .__/ \__,_|\__|                                                                                                                            
            |_|                                                                                                                                          
    */                                                                                                                                                   
                                                                                                                                                         
    data baseball;                                                                                                                                       
          length url $72 name $44;                                                                                                                       
          set sashelp.baseball(keep=name team league division obs=10);                                                                                   
          url = cats('https://www.google.com/search?q=', urlencode(strip(name)));                                                                        
    run;                                                                                                                                                 
                                                                                                                                                         
                                                                                                                                                         
    WORK.BASEBALL total obs=10                                                                                                                           
                                                                                                                                                         
         TEAM            LEAGUE     DIVISION                             URL                            NAME                                             
                                                                                                                                                         
       Cleveland      American      East       https://www.google.com/search?q=Allanson,%20Andy       Allanson, Andy                                     
       Houston        National      West       https://www.google.com/search?q=Ashby,%20Alan          Ashby, Alan                                        
       Seattle        American      West       https://www.google.com/search?q=Davis,%20Alan          Davis, Alan                                        
       Montreal       National      East       https://www.google.com/search?q=Dawson,%20Andre        Dawson, Andre                                      
       Montreal       National      East       https://www.google.com/search?q=Galarraga,%20Andres    Galarraga, Andres                                  
       Oakland        American      West       https://www.google.com/search?q=Griffin,%20Alfredo     Griffin, Alfredo                                   
       Montreal       National      East       https://www.google.com/search?q=Newman,%20Al           Newman, Al                                         
       Kansas City    American      West       https://www.google.com/search?q=Salazar,%20Argenis     Salazar, Argenis                                   
       Atlanta        National      West       https://www.google.com/search?q=Thomas,%20Andres       Thomas, Andres                                     
       Cleveland      American      East       https://www.google.com/search?q=Thornton,%20Andre      Thornton, Andre                                    
                                                                                                                                                         
    /*           _               _                                                                                                                       
      ___  _   _| |_ _ __  _   _| |_                                                                                                                     
     / _ \| | | | __| `_ \| | | | __|                                                                                                                    
    | (_) | |_| | |_| |_) | |_| | |_                                                                                                                     
     \___/ \__,_|\__| .__/ \__,_|\__|                                                                                                                    
                    |_|                                                                                                                                  
    */                                                                                                                                                   
                                                                                                                                                         
     d:\xls\hyperlink.xlsx                                                                                                                               
                                                                                                                                                         
       ----- ---------------------------------------------------------------------------------------------------------------                             
       |    |Division  League                                                                           Click to Google Se|                              
       | 1  |at the    at the                                                                           arch on Name      |                              
       |    |End of    End of    Team at the                                                            (using STYLE as   |                              
       |    |1986      1986      End of 1986     URL                                                    2nd argument)     |                              
       |----|-------------------------------------------------------------------------------------------------------------|                              
       | 2  |East    | American| Cleveland     | https://www.google.com/search?q=Allanson,%20Andy     | Allanson, Andy    |  * hiperliks in blue         
       |----|        |         |               |------------------------------------------------------+-------------------|  * click on name for google  
       | 3  |        |         |               | https://www.google.com/search?q=Thornton,%20Andre    | Thornton, Andre   |                              
       |----|        |---------+---------------+------------------------------------------------------+-------------------|                              
       | 4  |        | National| Montreal      | https://www.google.com/search?q=Dawson,%20Andre      | Dawson, Andre     |                              
       |----|        |         |               |------------------------------------------------------+-------------------|                              
       | 5  |        |         |               | https://www.google.com/search?q=Galarraga,%20Andres  | Galarraga, Andres |                              
       |----|        |         |               |------------------------------------------------------+-------------------|                              
       | 6  |        |         |               | https://www.google.com/search?q=Newman,%20Al         | Newman, Al        |                              
       |----|--------+---------+---------------+------------------------------------------------------+-------------------|                              
       | 7  |West    | American| Kansas City   | https://www.google.com/search?q=Salazar,%20Argenis   | Salazar, Argenis  |                              
       |----|        |         |---------------+------------------------------------------------------+-------------------|                              
       | 8  |        |         | Oakland       | https://www.google.com/search?q=Griffin,%20Alfredo   | Griffin, Alfredo  |                              
       |----|        |         |---------------+------------------------------------------------------+-------------------|                              
       | 9  |        |         | Seattle       | https://www.google.com/search?q=Davis,%20Alan        | Davis, Alan       |                              
       |----|        |---------+---------------+------------------------------------------------------+-------------------|                              
       |10  |        | National| Atlanta       | https://www.google.com/search?q=Thomas,%20Andres     | Thomas, Andres    |                              
       |----|        |         |---------------+------------------------------------------------------+-------------------|                              
       |11  |        |         | Houston       | https://www.google.com/search?q=Ashby,%20Alan        | Ashby, Alan       |                              
       --------------------------------------------------------------------------------------------------------------------                              
                                                                                                                                                         
    [hiperlink]                                                                                                                                          
                                                                                                                                                         
    GOOGLE RESUTLS WHEN YOU CLICK ON THE CELL WITH "ALLANSON, ANDY"                                                                                      
    ===============================================================                                                                                      
                                                                                                                                                         
    If you click on the cell with "Allanson, Andy"                                                                                                       
                                                                                                                                                         
    Google                                                                                                                                               
    Allanson, Andy                                                                                                                                       
                                                                                                                                                         
    About 125,000 results (0.53 seconds)                                                                                                                 
    Search Results                                                                                                                                       
    Web results                                                                                                                                          
                                                                                                                                                         
    Andy Allanson Stats | Baseball-Reference.comwww.baseball-reference.com › MLB Players › A Listing                                                     
    Jul 31, 2020 - Andy Allanson. Position: Catcher. Bats: Right • Throws: Right. 6-5, 220lb                                                             
    (196cm, 99kg). Born: December 22, 1961 (Age: 58-223d) in Richmond ...                                                                                
                                                                                                                                                         
    /*                                                                                                                                                   
     _ __  _ __ ___   ___ ___  ___ ___                                                                                                                   
    | `_ \| `__/ _ \ / __/ _ \/ __/ __|                                                                                                                  
    | |_) | | | (_) | (_|  __/\__ \__ \                                                                                                                  
    | .__/|_|  \___/ \___\___||___/___/                                                                                                                  
    |_|                                                                                                                                                  
    */                                                                                                                                                   
                                                                                                                                                         
    ods listing close;                                                                                                                                   
    Ods escapechar="^";                                                                                                                                  
    ods excel file="d:\xls\hyperlink.xlsx"                                                                                                               
          style=statistical                                                                                                                              
          options (wraptext="no" flow="tables" sheet_name="hiperlinks" );                                                                                
                                                                                                                                                         
    options FORMCHAR="|----|+|---+=|-/\<>*";                                                                                                             
    proc report data=baseball spanrows split='/' ;                                                                                                       
      column division league team url name;                                                                                                              
      define division / order;                                                                                                                           
      define league / order;                                                                                                                             
      define team / order;                                                                                                                               
      define url / display ;                                                                                                                             
      define name/display 'Click to Google Search on Name/(using STYLE as 2nd argument'                                                                  
             style={protectspecialchars=off};                                                                                                            
      compute name;                                                                                                                                      
         ** using 'STYLE' as 2nd argument and precalc URL with STYLE= as 3rd argument;                                                                   
         length svar $120;                                                                                                                               
           svar = catt('style={foreground=blue url="',url,'"}');                                                                                         
           call define(_col_,'style',svar);                                                                                                              
      endcomp;                                                                                                                                           
    quit;                                                                                                                                                
    ods excel close;                                                                                                                                     
    ods listing;                                                                                                                                         
                                                                                                                                                         
                                                                                                                                                         
