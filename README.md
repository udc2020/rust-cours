# Rust Course 🔥
## By: ***Ultrasdzcoder***
### You Can See Full Course [here](https://www.youtube.com/c/UltrasDzCoder?sub_confirmation=1)

---

## install Rust 

         curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh


## in editor
         cargo init
         cargo run


## Hello World 

         fn main(){
            println!("Hello World!");
         }

## Printing 
         
         // Use println! to show content in console
         println!("hi there !");

         // Use argument in print to add dynamic values
         println!("{} , {}","foo","bar");
         println!("{1} , {0}","bar","foo");
         println!("{foo} , {bar}",bar= "bar",foo="foo");


## Vars
         // we can use let , const
         // ! let
         let name = "udc";
         println!("my name is {}",name);

         // if we change name to ultrasdzcoder
         name = "ultrasdzcoder";// erro  this var is immutable (cant changed)

         // to make it muttable
         let mut name = "udc";
         println!("my name is {}",name);

         // now change the value
         name = "ultrasdzcoder";
         println!("my name is {}",name);

         //! const
         // most be name uppercase & declaering which type
         const PI :f32 = 3.14;
         println!("PI {}",PI);

         //! multiple vars
         let (name,age) = ("udc",26);
         println!("name : {} age : {}",name,age);


## Data Types

         /*
         int : (u) unsined integer <0,+@@> and (i) integer < -@@ , +@@> (8,16,32,64,128)
         floats : f (32,64)
         boolean : (true,false)
         characters : ("a","b"....)
         tuples :(1,"a",true)
         array : [html,css,rust]
         */

         let age = 26;// i32/i64 (548766464) >
         let udc_first_latter = 'u'; // most be one characters
         let phy:f32 =  1.64;// most have float point
         let is_alive = true; //(true or false)

         println!("{:?}",(age,udc_first_latter,phy,is_alive));


## Strings
         // has no data type named string
         // string is list of chars
         let loriem = "lorem ipsume...";
         println!("{}",loriem);

         //! Crearte String
         let mut str = String::from("that is real String ");
         println!("{}",str);
         //!  Add new charactres
         str.push('2');
         println!("{}",str);
         //!  Add new word
         str.push_str("022");
         println!("{}",str);
         //!  Get length
         println!("{}",str.len());

## Tuples
         // tuples like lists but it have many data types combain it
         //  most declear the type of all elements
         let person:(&str,&str,i8) = ("udc","ultrasdzcoder",26);
         // we can accsassing the tuple by use her index (tuple.index(int))
         println!("{:?}",(person.0,person.1,person.2));

## Arrays
         //  arrays is fixed length & have the same data type in his elements
         let arr:[i16;10] = [0,1,2,3,4,5,6,7,8,9];
         
         //! show all elements
         println!("{:?}",arr);

         //! get element by index
         println!("first element :{} last element :{}",arr[0],arr[9]);

         //! change the values of array
         let mut arr:[i8;4] = [2,5,4,6];
         arr[0] = 3;
         arr[1] = arr[2];
         arr[2] = 5;
         println!("{:?}",arr);

         //! length of array
         println!("{}",arr.len());

## Control Flow
         //! if/else
         let age:i32 = 12;

         // we can use if / else / else if

         if age > 18 {
            println!("You Have {}",age);
         }else if age < 15 {
            println!("you are child");
         }else{
            println!("you are under 18");
         }

         //! short hand if
         let humen = false;
         let is_alive = if humen { "i'm alive" } else { "you are tree" };
         
         println!("{}",is_alive);

## Loops
         //! loop
          let mut count = 0;
         // infinite loop
         loop{
            println!("number : {}",count);
         // must use increament
             count +=1;
         //  we add stop condetion
             if count >= 10 { break; }
          }

         //! while
         // start
          let mut count  = 0;
         //  end
          while count <= 9 {
          println!("number : {}",count);
         // staps
          count += 1 ;
          }

         //! for range
          for i in 0..10{
              println!("number : {}",i);
          }

## Functions
         //! import &  invoke the function  
         hello::say_hello(); // hello ultrasdzcoder

         //! call void function with args
         asking_name("udc");

         //! function with returnig type 
         println!("{}",add(10,15)); // 25
         
         //! Clasure short function
         let add  = |x:i32 , y:i32| x+y ; 
         println!("{}",add(10,15)); // 25



         
         // Void function
         // fn asking_name(name: &str) {
         //     println!("your name is {}", name);
         // }

         // function with returning type
         // fn add(x: i32, y: i32) -> i32 {
         //     x + y
         // }

         

