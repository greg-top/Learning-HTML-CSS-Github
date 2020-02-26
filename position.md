# Pozycjonowanie:
_daje możliwość manipulowania danego elementu nie zależnie od jego markapem._
### position: relative; ###  
*.klasa {
    position: relative;
    
    top: ;
    
    bottom:;
    
    left:;
    
    right:;
    
}*
- sama klasa z position relative nie wpływa na pozycje danego elementu.
- Po przesunięciu ustawia sie względem swojej pozycji starowej.
- Można wykorzystywać do przesuwania *transform: translateX/translateY(px)* 
### position: absolute; ###
_Sprawia że dany element wyskakuje z normalnego porządku na stronie._
*.klasa {*  
    *position: absolute;*  
    
    *top: ;*  
    
    *bottom:;*  
    
    *left:;*  
    
    *right:;*  
    
}*
- Można ustalać położenie danego elementu nie zależnie odjego markapu.
- Position:absolute pozycjonowane jest względem _*documents initial containing block*_ ma rozmiaru viewportu.
- Żeby ustawiać względem rodzica należy dodać do rodzica position:relative; np:

<style>
.box {  
    width:100px;  
    height:100px;  
}  
.container {  
    position:relative;  
    display:flex;  
    flex-wrap:wrap;  
}  
.absolute {  
    position:absolute;  
    bottom:0;  
    right:0;  
}  
</style>  
<body>  
    <div class="container">  
        <div class="box"></div>  
        <div class="box"></div>  
        <div class="box absolute"></div>  
        <div class="box"></div>  
        <div class="box "></div>  
    </div>  
</body>  
- Po takim zapisie *div* ustawi się w prawym dolnym rogu rodzica.

### position:fixed; ###
_Po nadaniu tej pozycji element zostaje przyklejony do strony, podczas skrolowania strony dany element pozostaje w nadanej mu pozycji._

### position:sticky; ###
_Należy pamietać że dana wartość nie jest należycie wspierana przez wszystkie przeglądarki,_
_W momęcie gdy element miał by wyjechać po za v-p zostaje w swoim miejscu._
