1. Run `rojo serve broken.project.json -vvv`.
2. Edit `src/hello.luau` and save. No Vfs event lines appear, and `http://localhost:34872/show-instances` keeps the old source until you restart Rojo.
3. Do the same with rojo serve `works.project.json -vvv`. Each save logs `Vfs event: Write(...)`, and the change syncs.
