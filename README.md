# kandinsky-api-requests

api для использования нейросети kandinsky 2.2

**Как использовать:**

### 1. text2image

```
async def main():
    test = FusionBrainApi()
    img_bytes = await test.text2image("Котик", style="CYBERPUNK")
    img = Image.open(img_bytes)
    img.save('cat_cyberpunk.jpg')


if __name__ == '__main__':
    asyncio.run(main())
```

Все стили можно посмотреть в `FusionBrainApi().styles`