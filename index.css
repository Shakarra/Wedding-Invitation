/* $('#husband_input').keyup(function(e){
  value = $(this).val()
  $('#husband_value').html(value)
})

$('#wife_input').keyup(function(e){
  value = $(this).val()
  $('#wife_value').html(value)
})

$('#lastname_input').keyup(function(e){
  value = $(this).val()
  $('#lastname_value').html(value)
})

$('#date_input').keyup(function(e){
  value = $(this).val()
  $('#date_value').html(value)
})

$('#location_input').keyup(function(e){
  value = $(this).val()
  $('#location_value').html(value)
}) */

function setInitials() {
  husbands_initial = $("#husband_input").val().trim()[0];
  wifes_initial = $("#wife_input").val().trim()[0];
  if(husbands_initial !== undefined && husbands_initial !== '' && wifes_initial !== undefined && wifes_initial !== '') {
    value = husbands_initial + ' & ' + wifes_initial;
    $('#initials_value').html(value)
  }
  else {
    $('#initials_value').html('')

  }
}

$("#husband_input").keyup(setInitials);


$("#wife_input").keyup(setInitials);

function checkBlank() {
  if( $('#husband_value').val() === undefined && $('#wife_value').val() === undefined) {
    $('#cordial').html('')
  }
  else {
    $('#cordial').html('cordially invite you to their wedding on')

  }
}

formfields= ['husband', 'wife', 'lastname', 'date', 'location']
function setKeyUpEvent(field){
  $('#' + field + '_input').keyup(function(e){
    checkBlank();
    value = $(this).val();
    $('#' + field + '_value').html(value)
    checkBlank()
  })
}
for(field of formfields){
    setKeyUpEvent(field)
}

$('.theme').click(function(e){
  $('.theme-link').removeClass('active')
  $(this).children(':first').addClass('active')
  id=$(this).attr('id')
  $('#invitation').removeClass('formal-theme')
    .removeClass('spring-theme')
    .removeClass('art-deco-theme')
    .addClass(id + '-theme')
})
