# Kagal Sergey

## Frontend developer

---

### Contacts

- [ ]  phone: +375 29 363 31 10
- [ ]  email: 3461995@gmail.com
- [ ]  tg: @Sergey_Kagal

### Skills

- [x]  HTML
- [x]  CSS
- [x]  JavaScript
- [x]  Git
---
### Code example:
```javascript
 simpleMove(from, to, dt, duration) {
    const result = [];
    let time = 0;
    this.posX = from.x;
    this.posY = from.y;
    result.push({ time: time, currentX: this.posX, currentY: this.posY });
    const deltaX = to.x - from.x;
    const deltaY = to.y - from.y;
    this.direction = getDirection(deltaX, deltaY);
    const distance = Math.sqrt(deltaY ** 2 + deltaX ** 2);
    this.speed = distance / duration;
    this.dx = Math.cos(this.direction) * this.speed * dt;
    this.dy = Math.sin(this.direction) * this.speed * dt;

    for (let time = dt; time <= duration; time += dt) {
      this.posX += this.dx;
      this.posY += this.dy;
      result.push({
        time: time,
        currentX: Math.round(this.posX),
        currentY: Math.round(this.posY),
      });
    }
    return result;
  }
```
