$(function() {
  $('.shopping-list-form').submit(event => {
    event.preventDefault();
    const userTextElement = $(event.currentTarget).find('#shopping-list-entry');
    $(".js-display-shopping-list-entry").text(`user text is:  ${userTextElement.val()}`);
    userTextElement.val("");
  });  
})


$(function() {
  $("button").click(function(event) {
  $('ul').appened
  }
})
