# Preprocesory CSS # 
* **Preprocesory CSS to narzędzia pozwalające tworzyć oraz utrzymywac arkusze stylów w sposób dużo lepiej zorganizowany, bardziej czytelny, prostszy, szybszy niż w standardowy sposób.**  
* **Dzięki temu, do dyspozycji są nowe, rozszerzone "abstrakcyjne" języki, które nie są jednak bezpośrednio rozumiane przez przeglądarki.**  
 *  _Preprocesory CSS rozumieją pisany "nowy" kod i dzięki temu potrafią go "przetłumaczyć" na kod CSS doskonale znany przeglądarkom._ 

 **_Abstrakcyjna warstwa na Przykładzie SASS:_**  

 // SASS stylesheet  
 $mainColor: #color;  
 $baseFont: rodzaj fontu;  

 body {  
     font:16px/22px $baseFont;  
     color: $mainColor;  
     text-shadow: 1px 1px 0 darken($mainColor, 80%);  
 }  

**_Wygenerowany kod CSS_**  

body{  
    font:16px/22px rodzaj fontu;  
    color: #color;  
    text-shadow: 1px 1px 0 black;  
}  

**Preprocesory CSS powstały:**  

* Aby rozszerzyć możliwości języka CSS, które nie oferuje **dynamicznych** cech znanych między innymi z języków programowania.  
* W myśl zasady **DRY** (Don't Repeat Yourself) - nie powtaraj się.  

## _Cechy języków programowania w arkuszach stylów to między innymi:_ ##  

* **zmienne** (ang.variables), do których można przypisywać wartości.  
* **domieszki/mixiny** (ang. mixins), jak szablony gotowe do wieloktotnego użycia.  
* **funkcje** (ang. functions), przyjmujące i zwracające wartości.  

**_przykład:_**  
**Standardowy kod CSS**  
#content p {  
    padding: 30px;   
    overflow: hidden;  
}  

#content p a {  
    color:#fff;  
}  

#content p a:hover {  
    color:#E6BE88;  
    text-decoration: underline;  
}

**Równoważny kod w LESS/SASS:**  
#content {  
    p {  
        padding: 30px;  
        overflow: hidden;  

        a {  
            color: #fff;  

        &:hover {
                color:#E6BE88;  
                text-decoration: underline;  
            }  
        }  
    }  
}  

### Najpopularniejsze preprocesory CSS ###
* LESS  
* SASS  
* Stylus  

