---
title: Lorem Ipsum
layout: post
author: Marcus Tullius Cicero
---
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed luctus, nunc laoreet porta volutpat, massa orci rutrum tellus, sit amet vestibulum libero enim id massa.

Nam semper urna sit amet metus auctor iaculis. Nam blandit, ante vitae vestibulum tristique, turpis ex faucibus diam, nec porttitor libero ex nec eros. Fusce ornare a neque sit amet congue.

```js
// Crappy code
ftpd.registerProcessor("isDir", (data: events.IsDirRequest, id, callback) => {
    const path = Path.join(base, data.path);
 
    callback(new events.IsDirResponse(fs.existsSync(path) && fs.lstatSync(path).isDirectory()));
});
 
ftpd.registerProcessor("readFile", (data: events.ReadFileRequest, id, callback) => {
    const path = Path.join(base, data.path);
 
    const from = fs.createReadStream(path, {flags:"r"});
    from.on("error", () => {
        callback(new events.Error());
    });
    from.on("end", function() {
        callback(new events.ReadFileResponse());
    });
 
    from.pipe(data.socket);
});
```

Vivamus in orci a quam vestibulum euismod. Donec blandit, tortor eget fermentum ultrices, diam augue ullamcorper massa, id condimentum orci magna sit amet velit. Pellentesque a facilisis lacus. Pellentesque a lectus nec ex efficitur interdum. Fusce interdum lorem nec neque dapibus, sit amet tempus metus vehicula.

![The San Juan Mountains are beautiful!](/images/2021-07-02-lorem-ipsum.jpg "San Juan Mountains")

Donec purus velit, auctor sit amet sodales vulputate, sagittis in eros. Pellentesque elit arcu, viverra et pharetra ac, condimentum nec sapien. Etiam ultricies lorem id laoreet eleifend. Duis malesuada felis vitae condimentum aliquet. Nunc sodales congue lacinia. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vivamus finibus velit sed felis dictum, sit amet laoreet tellus iaculis. Duis posuere efficitur elit eu consequat. Pellentesque vitae nisi gravida leo gravida gravida. Pellentesque congue purus diam, in bibendum sapien hendrerit sit amet. Fusce eu condimentum ante. Nullam hendrerit ipsum et felis consectetur, vitae hendrerit massa sagittis. Fusce sodales nunc id imperdiet efficitur. Aenean mattis laoreet magna, sed tincidunt nulla laoreet ut. Sed rutrum egestas orci non commodo. Aliquam egestas eros ac vehicula sollicitudin.