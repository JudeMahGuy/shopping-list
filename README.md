$(function() {
  $('#js-shopping-list-form').submit(event => {
    event.preventDefault();
    const userTextElement = $(event.currentTarget).find('#shopping-list-entry');
    $(".shopping-list").append('<li>' + 'shopping-list-entry.val()');
    userTextElement.val("");
  });  
})
  
  $('.shopping-list').on('click', '.shopping-item-delete', function(event) {
    this.remove();

$('.js-lightbulb').on('click', event => {
    // save reference to this bulb,
    const targetBulb = $(event.currentTarget);
    // and reference to all other bulbs
    const otherBulbs = $('.js-lightbulb').not(targetBulb);
    // store whether this bulb is aria-pressed.
    // because attr() returns strings, we convert it
    // back to a boolean by making a comparison.
    const pressedBool = $(targetBulb).attr('aria-pressed') === 'true';
    
    // Remove 'bulb-on' and uncheck bulbs that are not this one
    otherBulbs.removeClass('bulb-on').attr('aria-pressed', false);
    // toggle the presence of 'bulb-on' on this bulb; 
    // toggle aria-pressed by inverting pressedBool 
    // using the ! operator.
    targetBulb.toggleClass('bulb-on').attr('aria-pressed', !pressedBool);
  });
}

$(handleBulbClicks);
