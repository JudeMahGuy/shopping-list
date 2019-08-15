$(function() {
  $('#js-shopping-list-form').submit(event => {
    event.preventDefault();
    const userTextElement = $(event.currentTarget).find('#shopping-list-entry');
    $(".shopping-list").append('<li>' + 'shopping-list-entry.val()');
    userTextElement.val("");
  });  
})
  
  $('.shopping-list').on('click', 'li', function(event) {
    this.remove();


$(function() {
  $("button").click(function(event) {
  $('ul').appened
  }
})
