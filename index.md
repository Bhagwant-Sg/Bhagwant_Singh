<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thesis</title>
    <!-- <link rel="stylesheet" href="http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.css" />
    <script src="http://code.jquery.com/jquery-1.11.1.min.js"></script>
    <script src="http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.js"></script> -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Share+Tech&display=swap" rel="stylesheet">
    <style>
        body{
            font-family: 'Share Tech', sans-serif !important;
            background-image: url(Assets/Images/bg-main.png);
            background-attachment: scroll;
            background-repeat: no-repeat;
            background-position: 50% 0%;
            background-size: cover;
        }

        .jumbotron.top_jbtrn_sec {
            background: #FFFFFF;
            margin-top: 30px;
            padding: 30px 20px 30px 20px;
            text-align: center;
        }

        .jumbotron.top_jbtrn_sec h2 {
            font-size: 40px;
            text-transform: uppercase;
            color: #149414;
            font-weight: bolder;
        }
        
        .input-group.srch_br_cst input {
            padding: 10px 0px 10px 20px;
            height: 50px;
            border-radius: 6px;
        }

        .input-group.srch_br_cst.input-group-btn button {
            height: 50px !important;
        }

        button.btn.btn-default.cstm_btn\+_src_sq {
            height: 50px;
            border-top-right-radius: 6px;
            border-bottom-right-radius: 6px;
            background: #149414;
            color: #FFFFFF;
            font-size: 16px;
            padding: 2px 15px 0px 15px;
        }

        ul.list-group.cstm_list img {
            border: .09rem solid #149414;
            border-radius: 5px;
        }

        ul.list-group.cstm_list a {
            padding-left: 10px;
            font-size: 16px;
            color: #149414;
        }

    </style> 
</head>
<body>
    <!-- <div data-role="page">
        <div data-role="header">
            <h1>Project Thesis</h1>
        </div>

        <div data-role="main" class="ui-content">
            <ul data-role="listview" data-filter="true" data-filter-reveal="true">
                <li><a href="#">Lorem</a></li>
                <li><a href="#">Ipsum</a></li>
                <li><a href="#">Dolar</a></li>
            </ul>
        </div>

        <div data-role="footer" style="text-align: center;">
            <p>&copy; All Rights Reserved</p>
        </div>
    </div> -->

    <div class="container">
        <div class="jumbotron top_jbtrn_sec ">
            <h2>Project</h2>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quisquam facere debitis quod aliquam quam inventore sapiente quaerat fugit cupiditate recusandae?</p>
        </div>
        <div class="input-group srch_br_cst">
        <input class="form-control" id="myInput" type="text" placeholder="Search..">
        <div class="input-group-btn">
            <button class="btn btn-default cstm_btn+_src_sq" type="submit">
              <i class="glyphicon glyphicon-search"></i>
            </button>
          </div>
        </div>
        <br>
        <ul class="list-group cstm_list" id="myList">
            <li class="list-group-item">
                <img src="Assets/Images/Bhagwant.jpg" alt="" height="60px" width="60px">
                <a href="Files/Bhagwant-Portfolio/index.html">
                 Bhagwant Singh
                </a>
            </li>
            <li class="list-group-item">
                <img src="Files/Ransomware/Assets/Images/ransomware.png" alt="" height="60px" width="60px">
                <a href="Files/Bhagwant-Portfolio/index.html">
                 Ransomware Tester
                </a>
            </li>
            <li class="list-group-item">
                <img src="Files/PUP/Assets/Images/Pup_logo.png" alt="" height="60px" width="60px">
                <a href="Files/PUP/Assets/">
                 Punjab University Patiala
                </a>
            </li>
            <li class="list-group-item">
                <img src="Assets/Images/placeholder.png" alt="" height="60px" width="60px">
                <a href="Files/Bhagwant-Portfolio/index.html">
                 Bhagwant Singh
                </a>
            </li>                        
        </ul>
    </div>


    <script>
        $(document).ready(function(){
        $("#myInput").on("keyup", function() {
            var value = $(this).val().toLowerCase();
            $("#myList li").filter(function() {
            $(this).toggle($(this).text().toLowerCase().indexOf(value) > -1)
            });
        });
        });
    </script>

</body>
</html>
