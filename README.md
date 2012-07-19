# jQuery Live Search

Simple live search for content on web pages.

## Usage

    $('input[name="q"]').search('.searchable', function(on) {
      on.reset(function() {
        $('.searchable').show();
      });

      on.empty(function() {
        $('#empty-message').show();
      });

      on.results(function(results) {
        $('.searchable').hide();
        results.show();
      });
    });

View the example at http://nakajima.github.com/jquery-livesearch/
