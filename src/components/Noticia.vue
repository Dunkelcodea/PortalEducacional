<template>
<div class="p-4">
    <b-media>
  <img src="https://conceptodefinicion.de/wp-content/uploads/2014/09/School.jpg" alt="Responsive image">
  <h3>Titulo</h3>
  <p>asdjasdajsdkja sdkjhasdkjahsdkjahs dkjahssdkjah skdjhaskdjh aksdjhaksjdhaksdjasd Cras sit amet nibh libero, in   gravida nulla. Nulla vel metus scelerisque ante sollicitudin. Cras purus odio, vestibulum in vulputate at, tempus    viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.
   Donec sed odio dui. Nullam quis risus eget urna mollis ornare vel eu leo. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.</p>
    </b-media>
</div>
</template>


<style>

img{
  float:right;
  height:150px;
  padding:2px;
}


@media (max-width: 600px) {
  img{
    width:100%;

  }
}

</style>

<script>


export default {
  name: 'noticia',

}
</script>
