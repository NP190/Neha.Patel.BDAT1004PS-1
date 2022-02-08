Neha.Patel.BDAT1004PS#1
5      =integer
5.0    =float
5>1    =boolean
'5'    =string
5*2    =integer
5==3   =boolean
'5'*2  =string
'5'+'2'=string
5/2    =float
5%2    =float
{5,2,1}=list
pi(the no.)=float
```


Neha.Patel.BDAT1004PS#2
 string a = "Supercalifragilisticexpialidocious";
            Console.WriteLine("\nThe given string is:"+a);
            Console.WriteLine("\nTotal letters in the string are:" + a.Length);
            Console.WriteLine("\nDoes 'Supercalifragilisticexpialidocious' contain 'ice' as a substring:"+a.Contains("ice"));

            string b = "Honorificabilitudinitatibus";
            string c = "Bababadalgharaghtakamminarronnkonn";
            string longest; 
            if(a.Length>b.Length)
            {
                if(a.Length>c.Length){
                    longest = a;

                }
                else
                {
                    longest = c;
                }
            }
            else if(b.Length>c.Length)
            {
                longest = b;
            }
            else
            {
                longest = c;
            }
            Console.WriteLine("\nLongest string from "+a+ " ,"+b+" ,"+c+" is:-"+longest);
            string composer1 = "Berlioz";
            string composer2 = "Borodin";
            string composer3 = "Brian";
            string composer4 = "Bartok";
            string composer5 = "Bellini";
            string composer6 = "Buxtehude";
            string composer7 = "Bernstein";
            var composers = new List<string> { composer1, composer2, composer3, composer4, composer5, composer6, composer7};
            Console.WriteLine("SortedList of " + composer1+" ," + composer2+" ," + composer3+" ," + composer4+" ," + composer5+" ," + composer6+" ," + composer7);
             composers.Sort();
            foreach(var item in composers)
            {
                Console.WriteLine(item);

            }
```

    
    The given string is:Supercalifragilisticexpialidocious
    
    Total letters in the string are:34
    
    Does 'Supercalifragilisticexpialidocious' contain 'ice' as a substring:True
    
    Longest string from Supercalifragilisticexpialidocious ,Honorificabilitudinitatibus ,Bababadalgharaghtakamminarronnkonn is:-Bababadalgharaghtakamminarronnkonn
    SortedList of Berlioz ,Borodin ,Brian ,Bartok ,Bellini ,Buxtehude ,Bernstein
    Bartok
    Bellini
    Berlioz
    Bernstein
    Borodin
    Brian
    Buxtehude
    

Neha.Patel.BDAT1004PS#3
            int firstLength=6;
            int secondlength=7;
            int thirdlength=8;
            
            double s=(firstLength+secondlength+thirdlength)/2;
            double x=s*(s-firstLength)*(s-secondlength)*(s-thirdlength);
            double area = Math.Sqrt(x);
            
            Console.WriteLine("Area of triangle is: "+area);
         
           
```

    Area of triangle is: 15.491933384829668



Neha.Patel.BDAT1004PS#4
             
           int[] number={ 8, 55, 16,2, 9 };  
          
        foreach (var result in  number)  
        {  
            if (result % 2 == 0)  
            {  
                Console.WriteLine(result + " is Even  number");  
            }  
            else  
            {  
                Console.WriteLine(result + " is Odd  number");  
            }  }
```

    8 is Even  number
    55 is Odd  number
    16 is Even  number
    2 is Even  number
    9 is Odd  number
    


```Neha.Patel.BDAT1004PS#5
Console.WriteLine("Enter the sides of rectagle(x,y,x1,y1,x2,y2)");
            Console.Write("x=");
            string x = Console.ReadLine();
            Console.Write("y=");
            string y = Console.ReadLine();
            Console.Write("x1=");
            string x1 = Console.ReadLine();
            Console.Write("y1=");
            string y1 = Console.ReadLine();
            Console.Write("x2=");
            string x2 = Console.ReadLine();
            Console.Write("y2=");
            string y2 = Console.ReadLine();
            int X = 0;
            int Y = 0;
            int X1 = 0;
            int Y1 = 0;
            int X2 = 0;
            int Y2 = 0;

            try
            {
                X = Convert.ToInt32(x);
                Y = Convert.ToInt32(y);
                X1 = Convert.ToInt32(x1);
                Y1 = Convert.ToInt32(y1);
                X2 = Convert.ToInt32(x2);
                Y2 = Convert.ToInt32(y2);
            }
            catch
            {
                Console.WriteLine("Please enter only integer value");
            }
            if (X > X1 && X < X2 && Y > Y1 && Y < Y2)
            {
                Console.WriteLine("True");
            }
            else
            {
                Console.WriteLine("False");
            }
```

    Enter the sides of rectagle(x,y,x1,y1,x2,y2)
    x=y=x1=y1=x2=y2=False
    
