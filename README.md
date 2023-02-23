# AdrianoFappone.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <input placeholder="inserisci numero da dividere">
    <button style="padding: 10px; border-radius: 26px; background-color: red; color: black; cursor: pointer;">calcola i divisori</button>
    <h1 style="display: block;"></h1>
    <script>
        let bottone=document.querySelector('button')
        let lato=document.querySelector('input')
        let h1=document.querySelector('h1')
        bottone.onclick=function(){
            let valori=[]
            for(let i=0; i<lato.value; i++){
            if(lato.value%i==0){
                valori.push(i)
            }
            }
            if(valori.join("")!=1){
                h1.innerHTML=`i valori sono=${valori.join(", ")}`
            }
            else{
                h1.innerHTML=`è un numero primo`
            }
        }

    </script>
</body>
</html>
