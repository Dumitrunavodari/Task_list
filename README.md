<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-eOJMYsd53ii+scO/bJGFsiCZc+5NDVN2yr8+0RDqr0Ql0h+rP48ckxlpbzKgwra6" crossorigin="anonymous">

    <title>Hello, world!</title>
    <link rel="stylesheet" href="https://maxst.icons8.com/vue-static/landings/line-awesome/line-awesome/1.3.0/css/line-awesome.min.css">
  </head>
  <body>
    <div class="container">
      <div class="lista">
      </div>
      <div class="card">
        <div class="card">
          <h5>Adauga un task</h5>
        </div>
        <form>
          <div class="mb-3"> <!-- textul -->
            <label>Descriere</label>
            <input type="text" class="form-control" id="task">
          </div>
          <div class="mb-3 form-check"> <!-- checkbox -->
            <input type="checkbox" class="form-check-input" id="exampleCheck1">
            <label class="form-check-label" for="exampleCheck1">Urgent?</label>
          </div>
          <button type="submit" class="btn btn-primary" onclick="return adaugareTask();">Adauga</button>
        </form>
      </div>
    </div>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/js/bootstrap.bundle.min.js" integrity="sha384-JEW9xMcG8R+pH31jmWH6WWP0WintQrMb4s7ZOdauHnUtxwoG2vI5DkLtS3qm9Ekf" crossorigin="anonymous"></script>
    <script src='http://ajax.aspnetcdn.com/ajax/jQuery/jquery-3.2.1.js'></script>
    <script>
      function adaugareTask() {
        var task = $('#task').val();
        $(#'lista').append('
        <div class="card">
          <div class="card-body">
            <div class="card-body">
              <h5> ' + task +'</h5>
            </div>
          </div>
          <div class="card-footer text-muted">
            <a href="#" class="btn btn-danger"><i class="las la-trash"></i></a>
          </div>
        </div>')
        return false;
      }
    </script>
  </body>
</html>
