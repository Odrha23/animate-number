# animate-number
Animate list number like page rank

Used:

    <div id="data-count"><span class="count">100</span></div>
    <div id="data-count"><span class="count">87</span></div>

    <script>
    $('.count').each(function () {
        $(this).prop('Counter',0).animate({
            Counter: $(this).text()
        }, {
            duration: 8000,
            easing: 'swing',
            step: function (now) {
                $(this).text(Math.ceil(now));
            }
        });
    });      
    </script>
