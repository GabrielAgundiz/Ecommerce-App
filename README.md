# Ecommerce-App
<p>Durante el desarrollo de esta aplicación, pudimos experimentar de primera mano las ventajas y desafíos de trabajar con <em>isolates</em> en Dart para consumir una API REST. Los <em>isolates</em> nos permitieron realizar la obtención de datos de manera asíncrona, evitando que la interfaz de usuario se congelara mientras esperábamos la respuesta del servidor. Esto fue especialmente beneficioso al cargar los productos de la tienda en línea falsa proporcionada por "FakeStoreAPI".</p>

<p>Utilizar la biblioteca <code>http</code> de Dart facilitó en gran medida el consumo de la API REST. Mediante métodos como <code>get</code>, pudimos interactuar con los <em>endpoints</em> y obtener los datos de los productos en formato JSON. Sin embargo, decodificar el JSON a objetos de Dart utilizables en la aplicación representó un desafío inicial que superamos gracias a las bibliotecas especializadas.</p>

<p>Una vez obtenidos los datos, manejar el estado de la aplicación para reflejar los cambios en la interfaz de usuario fue otra tarea importante. Optamos por utilizar <code>StatefulWidget</code> para gestionar el estado y asegurarnos de que la galería de productos se actualizara correctamente cuando se obtuvieran nuevos datos o se cambiaran los que se muestran inicialmente.</p>

<p>No obstante, enfrentamos algunas dificultades durante el proceso. Implementar los <em>isolates</em> requirió trabajar con cuidado para evitar problemas de concurrencia y garantizar la integridad de los datos compartidos entre el hilo principal y los <em>isolates</em>. Además, tuvimos que implementar lógica de manejo de errores para situaciones como fallos en la conexión, respuestas inesperadas del servidor o datos malformados provenientes de la API.</p>

<p>En general, esta experiencia nos permitió mejorar nuestra comprensión sobre el uso de <em>isolates</em> en Dart, el consumo de APIs REST y la importancia de manejar eficientemente el estado y los errores en una aplicación, brindando una experiencia fluida y confiable al usuario.</p>