## สร้าง class Person มี porperty ดังนี้
    - id เลขระบุ
    - name ชื่อ
    - Wishlist สิ่งของที่อยากได้

## โดยที่ method ดังนี้
    - constructor(name)
        - กำหนด id ให้เป็น running number(ใช้ static) 
        (แบบว่า ไม่ต้องรับมาค่ามาจาก constructor ให้เลขรันเพิ่มไปเอง) โดยเริ่มที่ 1
        - กำหนด name ชือ โดยมีค่าเริ่มต้นเป็น 'N/A'
        - ให้ Wishlist  โดยกำหนดค่าเริ่มต้นเป็น empty array
    - getId 
        - ให้ return id
    - getName
        - ให้ return name
    - getWishlist
        - ให้ return wislist
    - addWishlist(item)
        - เพิ่ม item เข้าไปใน Wishlist
        - ถ้า item เป็น null หรือ undefind ให้ return undefind
        - โดยต้อง return เป็นความยาวล่าสุดของ array Wishlist
    - removeWishlist(item)
        - ลบ item ออกโดยใช้ ชื่อ item 
        - ถ้า item เป็น null หรือ undefind ให้ return undefind
        - ถ้า item ที่จะลบไม่มีอยู่จริงให้ return "not found to remove"
        - โดยต้อง return ชื่อ item ที่สามารถลบได้
    - findWishlist(item)
        - ถ้า item เป็น null หรือ undefind ให้ return undefind
        - หา item ที่อยู่ใน array wishlist และให้ return ออกมาเป็น object {index: ตำแหน่งของ item, value: ชื่อ item}
        - ถ้าไม่เจอ item ให้ return "not found"
    - toString()
        - นำ id name และ wishlist แสดงออกมาทั้งหมด
