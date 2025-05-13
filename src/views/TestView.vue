<template>
    <div class="container-fluid">
        <h1>Three equal width columns</h1>
        <p>Note: Try to add a new div with class="col" inside the row class - this will create four equal-width columns.</p>
        <div class="row">
            <div class="col p-3 bg-primary text-white">.col</div>
            <div class="col p-3 bg-dark text-white">.col</div>
            <div class="col p-3 bg-primary text-white">.col</div>
        </div>
        <div class="row mt-2">
            <div class="col p-3 bg-primary text-white">.col</div>
            <div class="col p-3 bg-dark text-white">.col</div>
            <div class="col p-3 bg-primary text-white">.col</div>
        </div>
        <div class="row mt-2">
            <div class="col-sm-4 bg-primary">
                <div class="row mt-2">
                    <div class="col-sm-2 bg-primary text-white">.col</div>
                    <div class="col-sm-6 bg-dark text-white">.col</div>
                    <div class="col-sm-4 bg-primary text-white">.col</div>
                </div>
            </div>
            <div class="col-sm-8">
                <div class="row mt-2">
                    <div class="col-sm-4 bg-primary">
                        <label for="email" class="form-label">Email:</label>
                    </div>
                    <div class="col-sm-8">
                        <input type="email" class="form-control" id="email" placeholder="Enter email" name="email">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
  name: 'TestView'
}
</script>
