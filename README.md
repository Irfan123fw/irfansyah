# Irfansyah
<div class="p-10 flex flex-col space-y-3">
  <div class="relative w-full sm:w-1/2 bg-gray-200 rounded">
    <div style="width: 60%" class="absolute top-0 h-4 rounded shim-green"></div>
  </div>

  <div class="relative w-full sm:w-1/2 bg-gray-200 rounded">
    <div style="width: 80%" class="absolute top-0 h-4 rounded shim-blue"></div>
  </div>

  <div class="relative w-full sm:w-1/2 bg-gray-200 rounded">
    <div style="width: 100%" class="absolute top-0 h-4 rounded shim-red"></div>
  </div>
</div>

.shim-green {
  position: relative;
  overflow: hidden;
  background-color: rgba(0, 255, 0, 0.7);
}
.shim-green::after {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  transform: translateX(-100%);
  background-image: linear-gradient(
    90deg,
    rgba(233, 233, 233, 1) 0,
    rgba(233, 233, 233, 0.9) 50%,
    rgba(233, 233, 233, 0.8) 100%
  );
  animation: shimmer 2s ease-out infinite;
  content: "";
}

.shim-blue {
  position: relative;
  overflow: hidden;
  background-color: rgba(0, 155, 255, 0.7);
}
.shim-blue::after {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  transform: translateX(-100%);
  background-image: linear-gradient(
    90deg,
    rgba(233, 233, 233, 1) 0,
    rgba(233, 233, 233, 0.9) 50%,
    rgba(233, 233, 233, 0.8) 100%
  );
  animation: shimmer 2.5s ease-out infinite;
  content: "";
}

.shim-red {
  position: relative;
  overflow: hidden;
  background-color: rgba(255, 0, 0, 0.7);
}
.shim-red::after {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  transform: translateX(-100%);
  background-image: linear-gradient(
    90deg,
    rgba(233, 233, 233, 1) 0,
    rgba(233, 233, 233, 0.9) 50%,
    rgba(233, 233, 233, 0.8) 100%
  );
  animation: shimmer 3s ease-out infinite;
  content: "";
}

@keyframes shimmer {
  100% {
    transform: translateX(0%);
    opacity: 0;
  }
}





