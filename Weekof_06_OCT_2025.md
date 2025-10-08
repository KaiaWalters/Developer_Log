How array methods can be applied to traversing large json obkects and rverifying the existence of a value or provide a fallback path if that value does not exist. For the full example see: 

```

export function getText(path: string, fallback: string = ''): string {
  const keys = path.split('.')
  let current: any = textContent
  
  for (const key of keys) {
    if (current && typeof current === 'object' && key in current) {
      current = current[key]
    } else {
      return fallback
    }
  }
  
  return typeof current === 'string' ? current : fallback
}

```