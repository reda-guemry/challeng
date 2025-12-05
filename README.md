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
