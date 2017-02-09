# Test
<!DOCTYPE html>
<html>
<head>
<meta charset="ISO-8859-1">
<title>Insert title here</title>
<link rel="stylesheet"
	href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<script
	src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script
	src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<script
	src="https://maps.googleapis.com/maps/api/js?key=AIzaSyD5LWOi2wv_rEWXviskgorrdTncVmwoDqY&libraries=places"></script>

<style>
#map {
	height: 590px;
	border: 1px solid black;
}

#rightPanel {
	height: 590px;

	float: right;
	overflow: auto;
}
</style>
</head>
<body>
	<div class="container-fluid">
		<div class="panel panel-info">
			<div class="panel-heading">

				<div class="row">
					<div class="col-sm-7">
						<img src="Images/images1.jpg" width="40" height="40">
					</div>
					<div class="col-sm-5">
						<input type="text" class="input-sm" id="source"
							placeholder="Source"> <input type="text" class="input-sm"
							id="destination" placeholder="Destination"> <span
							class="btn-group">
							<button id="search_button" class="btn btn-info btn-sm">
								<span class="glyphicon glyphicon-search"></span> Search
							</button>
							<button class="btn btn-info dropdown-toggle btn-sm"
								data-toggle="dropdown">
								<span class="caret"></span>
							</button>
							<ul class="dropdown-menu ">
								<li><a href="#" id="getCurrentLoc" class="searchoptions">get
										current location</a></li>
								<li><a href="#" id="currentLocInSource"
									class="searchoptions">current location in source</a></li>
							</ul>
						</span>
					</div>
				</div>
			</div>
		</div>
		<div class="panel-body">
			<div class="row">
				<div class="col-sm-12">
					<div id="map"></div>
				</div>
				<div class="col-sm-5">
					<div id="rightPanel"></div>
				</div>
			</div>
		</div>
	</div>
			<script type="text/javascript" src="Map.js"></script>
</body>
</html>

$(".col-sm-12").removeClass("col-sm-12").addClass("col-sm-7");
