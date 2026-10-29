# Studio 3D Trace

Editor 3D berbasis Three.js (r160). Situs statis: tanpa build, siap deploy ke Vercel.

## Deploy
- `vercel --prod` dari folder ini, atau unggah folder ke Vercel (Framework: Other).
- Three.js, three-mesh-bvh, dan three-bvh-csg dimuat dari cdn.jsdelivr.net (versi dipin), jadi perlu internet.

## Fitur
- Trace gedung dan jalan dari gambar peta/screenshot; jalan bisa dihaluskan (lengkung) dan punya trotoar, kerb, marka.
- Gedung parametrik (lantai, jendela, balkon, pintu, parapet, dll), persimpangan T/Y/perempatan.
- Primitif, transform numerik, undo/redo, grup, array, cermin, boolean, lengkung (bend).
- Edit Mode titik/rusuk/sisi: extrude, inset, loop cut, hapus, gabung titik, balik normal.
- Autosave lokal; simpan/buka proyek .json; ekspor .glb/.obj/.stl/.png; impor .glb.

## Batasan
- Bukan 1:1 dengan Blender. Belum ada: bevel, sculpt, animasi, rigging, render, spline umum.
- Ekspor .obj/.stl tidak membawa detail instancing (jendela/pintu); gunakan .glb.
- Model .glb hasil impor tidak ikut autosave.
