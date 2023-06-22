@import url('https://fonts.googleapis.com/css2?family=Poppins:wgh@300;400;500;600;700;800;900&display=swap');

*
{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body
{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: #111;
}

h2
{
    position: relative;
    font-size: 6em;
    color: #222;
}

h2::before
{
    content: attr(data-text);
    position: absolute;
    color: #fff;
    width: 350px;
    overflow: hidden;
    white-space: nowrap;
    border-right: 4px solid #fff;
    animation: text-animation 8s linear infinite;
    filter: drop-shadow(0 0 20px #fff) drop-shadow(0 0 50px #fff);
}

@keyframes text-animation
{
    0%, 10%, 100%
    {
        width: 0;
    }
    70%, 90%
    {
        width: 100%;
    }
}

