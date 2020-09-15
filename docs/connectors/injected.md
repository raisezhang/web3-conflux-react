# `web3-conflux-react` Documentation - Injected

- [`web3-conflux-react` Documentation - Injected](#web3-conflux-react-documentation---injected)
  - [Install](#install)
  - [Arguments](#arguments)
  - [Example](#example)
  - [Errors](#errors)
    - [NoConfluxProviderError](#noconfluxprovidererror)
      - [Example](#example-1)
    - [UserRejectedRequestError](#userrejectedrequesterror)
      - [Example](#example-2)

## Install
`yarn add @web3-conflux-react/injected-connector`

## Arguments
```typescript
supportedChainIds?: number[]
```

## Example
```javascript
import { InjectedConnector } from '@web3-conflux-react/injected-connector'

const injected = new InjectedConnector({ supportedChainIds: [1, 2] })
```

## Errors

### NoConfluxProviderError

#### Example
```javascript
import { NoConfluxProviderError } from '@web3-conflux-react/injected-connector'

function Component () {
  const { error } = useWeb3React()
  const isNoConfluxProviderError = error instanceof NoConfluxProviderError
  // ...
}
```

### UserRejectedRequestError

#### Example
```javascript
import { UserRejectedRequestError } from '@web3-conflux-react/injected-connector'

function Component () {
  const { error } = useWeb3React()
  const isUserRejectedRequestError = error instanceof UserRejectedRequestError
  // ...
}
```
