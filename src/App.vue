<template>
	<div id="app">
		<div class="container">

		<!-- TITLE : START -->
		<div class="page-header">
			<h1>Project 01 - ToDo List <small>VueJs</small></h1>
			<hr class="my-4">
		</div>
		<!-- TITLE : END -->


		<div class="row">
			<!-- CONTROL (SEARCH + SORT + ADD) : START -->
			<div class="col-12 col-lg-6">
				<div class="row">
					<!-- SORT : START -->
					<div class="col-12">
						<div class="form-group">
							<div class="dropdown">
								<button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton"
									data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
									Sort by
								</button>
								<div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
									<a class="dropdown-item" href="#">Name ASC</a>
									<a class="dropdown-item" href="#">Name DESC</a>
									<div class="dropdown-divider"></div>
									<a class="dropdown-item" href="#">Level ASC</a>
									<a class="dropdown-item" href="#">Level DESC</a>
								</div>
								<span class="badge badge-success badge-medium">NAME - DESC</span>
							</div>
						</div>
					</div>
					<!-- SORT : END -->

					<!-- SEARCH : START -->
					<div class="col-12">
						<div class="input-group">
							<input type="text" class="form-control" placeholder="Search for..." />
							<span class="input-group-append">
								<button class="btn btn-info" type="button">Clear!</button>
							</span>
						</div>
					</div>
					<!-- SEARCH : END -->
				</div>
			</div>
			<!-- CONTROL (SEARCH + SORT + ADD) : END -->

			<!-- FORM : START -->
			<div class="col-12 col-lg-6">
				<!-- ADD : START -->
				<div class="form-group add-task">
					<button type="button" class="btn btn-info btn-block">Add Task</button>
				</div>
				<!-- ADD : END -->

				<form action="" method="POST" class="form-inline justify-content-between">
					<div class="form-group">
						<label class="sr-only" for="">label</label>
						<input type="text" class="form-control" placeholder="Task Name" />
					</div>
					<div class="form-group">
						<label class="sr-only" for="">label</label>
						<select name="ds" class="form-control" required="required">
							<option value="0">Small</option>
							<option value="1">Medium</option>
							<option value="2">High</option>
						</select>
					</div>

					<button type="button" class="btn btn-primary">Submit</button>
					<button type="button" class="btn btn-secondary">Cancel</button>
				</form>
			</div>
			<!-- FORM : END -->
		</div>

		<!-- LIST : START -->

		<div class="panel panel-success">
			<div class="panel-heading">List Task</div>
			<table class="table table-hover ">
				<thead>
					<tr>
						<th style="width: 10%" class="text-center">#</th>
						<th>Task</th>
						<th style="width: 20%" class="text-center">Level</th>
						<th style="width: 160px">Action</th>
					</tr>
				</thead>

				<tbody>
					<tr>
						<td class="text-center">1</td>
						<td>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis ea c</td>
						<td class="text-center"><span class="badge badge-danger">High</span></td>
						<td>
							<button type="button" class="btn btn-warning">Edit</button>
							<button type="button" class="btn btn-danger">Delete</button>
						</td>
					</tr>
					<tr>
						<td class="text-center">2</td>
						<td>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis ea c</td>
						<td class="text-center"><span class="badge badge-secondary">Small</span></td>
						<td>
							<button type="button" class="btn btn-warning">Edit</button>
							<button type="button" class="btn btn-danger">Delete</button>
						</td>
					</tr>
					<tr>
						<td class="text-center">3</td>
						<td>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis ea c</td>
						<td class="text-center"><span class="badge badge-info">Medium</span></td>
						<td>
							<button type="button" class="btn btn-warning">Edit</button>
							<button type="button" class="btn btn-danger">Delete</button>
						</td>
					</tr>
				</tbody>

			</table>
		</div>
	</div>
	</div>
</template>

<script>
export default {
	name: 'app',
	data () {
		return {
			
		}
	},
	components: {

	}
}
</script>

<style>
	#app {
		font-family: 'Avenir', Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		margin-top: 60px;
	}

	h1, h2 {
		font-weight: normal;
	}

	ul {
		list-style-type: none;
		padding: 0;
	}

	li {
		display: inline-block;
		margin: 0 10px;
	}

	a {
		color: #42b983;
	}
</style>
