# mini-j-highlight

    .___  ___.  __  .__   __.  __                 __          __    __   __    _______  __    __   __       __    _______  __    __  .___________.
    |   \/   | |  | |  \ |  | |  |               |  |        |  |  |  | |  |  /  _____||  |  |  | |  |     |  |  /  _____||  |  |  | |           |
    |  \  /  | |  | |   \|  | |  |  ______       |  |  ______|  |__|  | |  | |  |  __  |  |__|  | |  |     |  | |  |  __  |  |__|  | `---|  |----`
    |  |\/|  | |  | |  . `  | |  | |______|.--.  |  | |______|   __   | |  | |  | |_ | |   __   | |  |     |  | |  | |_ | |   __   |     |  |     
    |  |  |  | |  | |  |\   | |  |         |  `--'  |        |  |  |  | |  | |  |__| | |  |  |  | |  `----.|  | |  |__| | |  |  |  |     |  |     
    |__|  |__| |__| |__| \__| |__|          \______/         |__|  |__| |__|  \______| |__|  |__| |_______||__|  \______| |__|  |__|     |__|     
                                                                                                                                                
## Description

hilighter which work with every programming language in a best effort manner.

## About

  * best effort highlighter
  * minimal size
  * no language detection
    * may work with every programming language
    * use a fixed list of key-words
  * customizable with simples CSS
    * using attributes

## Exemples

### A SQL exemple :

    select * from toto
    where id > 42 ;

![With mini-j-highlight](/img/exemple_sql_001.png)
    
### A JS exemple : 

    import miniJHighlight from './mini-j-highlight.js';
    window.addEventListener('load', function(event) {
        document.querySelectorAll('[type="mini-j-highlight"]').forEach((e)=>{
            const container = document.createElement("div" );
            e.parentNode.insertBefore(container, e);
            e.style.display='none';
            miniJHighlight(container, e.innerText);
        });
    }); 

![With mini-j-highlight](/img/exemple_js_001.png)

### A Java exemple :

    /* Affichage console */
    public class HelloWorld {
        public static void main(String[] args) {
            System.out.println("Hello, world!"); 
        }
    }

![With mini-j-highlight](/img/exemple_java_001.png)
