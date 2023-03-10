<script lang="ts">

</script>

<div>
    <nav>
        <span class="logo">PANJEZIKU</span>
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
            margin-right: 250px;
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

</style>