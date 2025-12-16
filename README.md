challenge n1 for débutant  

//challeng number 11 : 

function sommeofarray(arr) {
    let res = arr.reduce((rep , ele) =>  rep+= ele ,0)
    console.log(res)
}


//challenge number 13 

function countVowels(str) {
    const check = ["a", "e", "i", "o", "u"]
    let res = 0 ; 
    for(let i = 0 ; i < str.length ; i++){
        if(check.includes(str[i])) {
            res += 1 ; 
        }
    }
    console.log(res) ; 
}

//challenge 15 : 
function isAlphanumeric(str) {
    const regex = /^[a-zA-Z0-9]+$/ ; 
    if(regex.test(str)) {
        console.log("true") 
    }else {
        console.log("false")
    }
}


challenge n2 for intermédiaire 

//challeng number 10:

function findLongestWord (tabl) {
    let temp = tabl.split(" ");
    console.log(temp)
    let res = temp[0]
    temp.forEach(ele => res.length > ele.length ? null : res = ele )
    console.log(res);
}

//challeng number 09:

function isPerfectNumber (num) {
    let fact = 0 ;
    for(let i = 1 ; i < num ; i++){
        if(num % i == 0) {
            fact += i 
        }
    }
    let res = fact == num 
    console.log(res)
}

//challeng number 02: 

function isPrime  (params) {
    let res = true ; 
    if(params <= 1){
        res = false ;
    }else {
        for(let i = 2 ; i < params ; i++){
            if(params % i == 0 ) {
                res = false ; 
            }
        }
    }
    console.log(res) ; 
}

challenge n3 for avancé  

//challenge 01 array 

const numbers = [1, 2, 3, 4, 5];
const sum = numbers.reduce((res , ele) => res += ele ,0)
console.log(sum); 



//challenge 02 array 

const duplicates = [1, 2, 2, 3, 4, 4, 5];
const unique = []
duplicates.forEach(ele => unique.includes(ele) ? null : unique.push(ele))
console.log(unique);


//challenge 03 array 

const numbers = [1, 3, 2, 5, 4];
const max =  numbers.reduce((res , ele) => res > ele ? res : res = ele ,0)
console.log(max); 


//challenge  19 avancé : 

function breadthFirstSearch( params , inde) {
    let rep = [] ;  
    rep.push(inde) ;
     for(let i = 0 ; i < rep.length ; i++ ) {
        params[rep[i]].forEach(ele => {
            if(!rep.includes(ele)){
                rep.push(ele)
            }
        }) 
    } 
    console.log(rep)
}

