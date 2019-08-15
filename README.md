$(function entry() {
  $('#js-shopping-list-form').submit(event => {
    event.preventDefault();
    const userTextElement = $(event.currentTarget).find('#shopping-list-entry');
    $(".shopping-list").append('<li>' + 'shopping-list-entry.val()');
    userTextElement.val("");
  });  
})
 
 $(function delete() {
  $('.shopping-list').on('click', '.shopping-item-delete', function(event) {
    this.remove();
});

$(function check() {
$('.shopping-item-toggle').on('click', event => {
    const targetItem = $(event.currentTarget);
    const pressedBool = $(targetItem).attr('aria-pressed') === 'true';
    targetItem.toggleClass('checked').attr('aria-pressed', !pressedBool);
  });
}
});

$(handleBulbClicks);
