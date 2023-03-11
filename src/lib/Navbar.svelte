<script lang="ts">

</script>

<div>
    <nav>
        <input type="checkbox" id="check">
        <label for="check" class="checkbtn">
            <i class="fas fa-bars"></i>
        </label>
        <span class="logo" id="logo">PANJEZIKU</span>
        <ul>
            <li><a href="#.com">Home</a></li>
            <li><a href="#.com">Workouts</a></li>
            <li><a href="#.com">Log</a></li>
            <li><a href="#.com">Contact</a></li>
        </ul>
    </nav>
</div>

<style lang="scss">
    *{
        text-decoration: none;
        list-style: none;
    }
    nav{
        background: #581414;
        height: 60px;
        width: 100%;
        .checkbtn{
            font-size: 30px;
            color: white;
            float: right;
            line-height: 60px;
            margin-right: 40px;
            cursor: pointer;
            display: none;
        }
        #check{
            display: none;
        }
        .logo{
            width: 300px;
            color: white;
            font-size: 35px;
            line-height: 60px;
            padding: 0 250px;
            font-weight: bold;
        }
        ul{
            float: right;
            margin-right: 10px;
            li{
                display: inline-block;
                line-height: 60px;
                margin: 0 10px;
                a{
                    color: white;
                    font-size: 17px;
                    text-transform: uppercase;
                    padding: 8px 15px;
                    border-radius: 3px;
                    &:hover{
                        background: #751c1c;
                        transition: ease-in-out .2s,;
                    }
                }
            }
        }

    }
    @media (max-width: 1152px){
        #logo{
            font-size: 25px;
            padding-left: 50px;
            padding-right: 50px;
        }
        nav ul li a{
            font-size: 16px;
        }
    }
    @media (max-width: 912px){
        .checkbtn{
            display: block !important;
        }
        ul{
            position: fixed;
            width: 100%;
            height: 100vh;
            background: #350c0c;
            left: -100%;
            text-align: center;
            transition: all .5s;
            z-index: 9999;
            opacity: 0.9;
        }
        nav ul li{
            display: block;
            a{
                font-size: 20px;
                &:hover,&:active{
                    background: none;
                    color: #751c1c;
                }
            }
        }
        #check:checked ~ ul{
            left: 0;
            
        }
    }
</style>