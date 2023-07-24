<div class="container">
		<div class="row">
			<div class="col-md-4 mx-auto">
				<form>
					<div class="form-group">
						<label for="exampleInputEmail1">Email address</label>
						<input type="search" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
						<small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
					</div>
					<div class="form-group" id="password">
						<label for="exampleInputPassword1">Password</label>
						<input type="password" class="form-control" id="exampleInputPassword1">
						<i class="fa fa-eye-slash"></i>
					</div>
					<div class="form-group form-check">
						<input type="checkbox" class="form-check-input" id="exampleCheck1">
						<label class="form-check-label" for="exampleCheck1">Check me out</label>
					</div>
					<button type="submit" class="btn btn-primary">Submit</button>
				</form>
			</div>
		</div>
	</div>
	<script>
		$(document).ready(function(){
			$('.fa-eye-slash').click(function(){
				$(this).toggleClass('fa-eye-slash');
				$(this).toggleClass('fa-eye')
			});
		});
	</script>
	<script>
		$('.fa-eye-slash').on('click', function(){
      $(this).text(function(){
        if($(this).text() === 'Hide'){
          $('#exampleInputPassword1').attr('type','password');
          return 'Show';
      } else {
          $('#exampleInputPassword1').attr('type','text');
          return 'Hide';
      }
    });
  });
	</script>
