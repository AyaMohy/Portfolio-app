<script>
export default{
    props:['title', 'desc', 'percent']
}
</script>
<template>
    <div>
        <div >
        <div class="row">
          <a
            class="text-decoration-none bg-transparent text-white col-2"
            data-bs-toggle="collapse"
            :href="`#${title}`"
            role="button"
            aria-expanded="false"
            aria-controls="collapseExample"
          >
            {{title}}
          </a>
          <div class="progress col-8 ps-0">
            <div
              class="progress-bar bg-success "
              role="progressbar"
              aria-label="Example with label"
              :style="{width: `${percent}%`}"
              aria-valuenow="30"
              aria-valuemin="0"
              aria-valuemax="100"
            >
              {{percent}}%
            </div>
          </div>
        </div>

        <!-- <div class="collapse border-0" :id="title">
          <div class="card card-body bg-transparent text-white border-0">
            {{desc}}
          </div>
        </div> -->
      </div> 
    </div>
</template>