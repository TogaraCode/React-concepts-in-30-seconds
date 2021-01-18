## Writing Your Own Hooks

### To customise Hooks we add the word use to the function. It allows components to share logic and check if changes are made in the state of a component and act accordingly.

## Example

```
index.js
```

```
import React from 'react';
import ReactDOM from 'react-dom';

function UserAccountStatus(props) {
  const isPremiumMember = useUserAccountStatus(props.user.id);

  if (isPremiumMember === null) {
    return 'Upgrade to Premium Membership available!';
  }
  return isPremiumMember ? 'PremiumMember' : 'Standard';
}

ReactDOM.render(<UserAccountStatus />, document.getElementById('root'));
```

## Screen View

### Upgrade to Premium Membership available!
