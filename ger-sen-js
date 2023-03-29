const generatePassword = (length) => {
    const charset = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!@#$%^&*()_+~`|}{[]\:;?><,./-=";
    let password = "";
    for (let i = 0, n = charset.length; i < length; ++i) {
      password += charset.charAt(Math.floor(Math.random() * n));
    }
    return password;
  };
  
  const button = document.querySelector("#generate");
  const input = document.querySelector("#length");
  const output = document.querySelector("#password");
  
  button.addEventListener("click", () => {
    const length = parseInt(input.value);
    const password = generatePassword(length);
    output.textContent = password;
  });
