<!DOCTYPE html>
<html>
    <head>
        <title>Hangman</title>
        <link  href="css/styles.css" rel="stylesheet" type="text/css" />
        <link href="https://fonts.googleapis.com/css?family=Pacifico" rel="stylesheet">
        <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
        
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
        
        <meta name="viewport" content="width=device-width, initial-scale=1">
    
        
    
    </head>
    <body>
        <div class='container text-center'>
            <header>
            <h1>Hangman</h1>
            </header>
            
            <div id="won">
                <h2>You Won!</h2>
                <button class="replayBtn btn btn-sucess">Play Again</button>
            </div>
            <div id="lost">
                <h2>You Lost!</h2>
                <button class="replayBtn btn btn-warning">Play Again</button>
            </div>
        
            <div id="word"></div>
            <div id="letters">
                <!--<input type="text" id="letterBox" size="3">-->
                <!--<button id="letterBtn">Submit</button>-->
            </div>
        
            <div id="man">
            <img src="img/stick_0.png" id="hangImg">
            </div>
        </div>
    </body>
    
    <script language="javascript">
        var selectedWord = "";
        var selectedHint = "";
        var hintshowen = false;
        var board = [];
        var remainingGuesses = 6;
        var words = [{word: "snake", hint: "It's a reptile"},
                     {word: "beetle", hint: "It's an insect"},
                     {word: "monkey", hint: "It's a mammal"},
                     {word: "horse", hint: "It's a mammal"},
                     {word: "whale", hint: "It's a fish"}];
        var alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 
                'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 
                'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z'];

        //alert("first word: " + words[0]); use alert to debug
        //console.log(words[0]);
        //console.log(selectedWord);
        
        //EVENTS
        
        //$("#letterBtn").click(function(){alert("hi")});
        $(".replayBtn").on("click", function(){
            location.reload();
        });
        
        startGame();
        
        function checkLetter(letter){
            var positions = new Array();
            for(var i = 0; i < selectedWord.length; i++){
                console.log(selectedWord)
                if(letter == selectedWord[i]){
                    positions.push(i);
                }
            }
            if(positions.length > 0){
                updateWord(positions, letter);
                if(!board.includes('_')){
                    endGame(true);
                }
            }
            else{
                remainingGuesses -= 1;
                updateMan();
            }
            if(remainingGuesses <= 0){
                endGame(false);
            }
        }
        function startGame(){
            pickWord();
            initBoard();
            updateBoard();
            createLetters();

        }
        function updateWord(positions, letter){
            for(var pos of positions){
                board[pos] = letter;
            }
            updateBoard();
        }
        function updateBoard(){
            $("#word").empty()
            for(var letter of board){
                document.getElementById("word").innerHTML += letter + " ";
                //$("#word").html();
            }
            $("#word").append("<br/>");
            if(hintshowen == false){
                $("#word").append("<button class='hintbtn'>Hint</button>");
            }
            $(".hintbtn").click(function(){
                $("#word").append("<span class='hint'>Hint: " + selectedHint + "</span>");
                remainingGuesses--;
                $(".hintbtn").hide();
                hintshowen = true;
            });
            if(hintshowen == true){
                $("#word").append("<span class='hint'>Hint: " + selectedHint + "</span>");
            }
            
        }
        function disableButton(btn){
            btn.prop("disabled", true);
            btn.attr("class", "btn btn-danger");
        }
        function updateMan(){
            $("#hangImg").attr("src", "img/stick_" + (6 - remainingGuesses) + ".png");
        }
        function endGame(win){
            $("#letters").hide();
            if(win){
                $('#won').show();
            }
            else{
                $('#lost').show();
            }
        }
        function pickWord(){
            var randomInt = Math.floor(Math.random()*words.length);
            selectedWord = words[randomInt].word.toUpperCase();
            selectedHint = words[randomInt].hint;
        }
        function createLetters(){
            for(var letter of alphabet){
                $("#letters").append("<button class='letter' id='"+letter +"'>"+ letter + "</button>");
                
            }
            $(".letter").click(function(){
                checkLetter($(this).attr("id"));
                disableButton($(this));
                console.log($(this).attr("id"));
            });
        }
        function initBoard(){
            for(var letter in selectedWord){
                board.push("_");
            }
        }
        console.log(board);
    </script>
    
    
</html>